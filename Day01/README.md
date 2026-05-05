## Role of Data Engineer:

1.Replicate and Migrate - Tasfer the Raw data into Google Cloud
2.Ingest - Raw data is available in a data source
3.Transform - Process the data using EL or ELT or ETL.
4.store - processed data is available in sink.

### Replicate and Migrate:

on-premis to google cloud
service like,
- gcloud storage (smaller size of data)
- Transfer Appliance (larger size of data)
- Storage Transfer Service (medium size of data)
- Datastream

## The Task level 1:

### sub-1
1.Launched the gcloud lab
2.opened BigQuery and created dataset named "nyctaxi"
3.create table in nyctaxi using fileformat of csv, table name: "2018trips"
4.used google console cmd,

```shell
bq load \
--source_format=CSV \
--autodetect \
--noreplace  \
nyctaxi.2018trips \
gs://cloud-training/OCBL013/nyc_tlc_yellow_trips_2018_subset_2.csv
```

to append the data into existing table.

### sub-2
1.Launched the gcloud lab
2.created sub table from existing table "2018trips" as january_trips

#standardSQL
CREATE TABLE
  nyctaxi.january_trips AS
SELECT
  *
FROM
  nyctaxi.2018trips
WHERE
  EXTRACT(Month
  FROM
    pickup_datetime)=1;

## The Task level 2:
