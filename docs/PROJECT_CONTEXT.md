# Project Context

## Problem

This project demonstrates Hadoop-era batch ETL using Apache Pig over search-query log data. The analytical theme is query popularity and temporal behavior: parse raw logs, derive useful fields, aggregate phrase frequency, compare time windows, and publish results to distributed storage.

## Data Engineering Flow

Raw query logs -> HDFS -> Pig LOAD -> parsing and filtering -> grouping -> aggregation -> STORE -> HDFS result validation.

## Domain Interpretation

The lab is a search/log analytics exercise. Frequency analysis can reveal common queries, temporal demand shifts, workload patterns, and candidate features for downstream analytics.

## Data Quality Questions

- Is the delimiter parsed correctly?
- Are timestamps converted consistently?
- Are empty queries removed?
- Are duplicate records expected or accidental?
- Are output paths versioned or cleared before reruns?

## Validation

Validate source counts, parsed records, intermediate relations, grouped counts, output directories, and sample output records.

## Use Cases

Batch log analytics, search analytics, ETL education, historical Hadoop migration studies, and conversion to Spark SQL, PySpark, Flink, Beam, EMR, Glue, or Databricks.

## Public-Artifact Standard

Use public or synthetic log data. Remove personal identifiers, account identifiers, private hostnames, internal paths, private network details, credentials, tokens, and organization-specific information before publication.
