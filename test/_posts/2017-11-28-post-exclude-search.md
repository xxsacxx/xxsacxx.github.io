---
title:  "How to move Partitioned Big Query Tables to AWS Athena"
search: true
categories: 
  - Jekyll
last_modified_at: 2020-06-04T08:05:34-05:00
---

There are so many awesome articles explaining stepwise execution for the flow of data from AWS setup to GCS like :
[from s3 to gcp](https://cloud.google.com/solutions/transferring-data-from-amazon-s3-to-cloud-storage-using-vpc-service-controls-and-storage-transfer-service)
But I faced some troubles while doing the other way around. It took me a few hours to properly setup. So I thought of sharing my work which might end up saving you some time.
Here is the GitHub repo :
[from s3 to gcp](https://github.com/xxsacxx/bq2s3)

After this, you will have an understanding of:
- How to work with partitioned tables in Big Query
- Moving partitioned tables from Big Query to GCS
- Exporting avro file from GCS to S3
- Getting the schema file from avro file
- Converting avro data to parquet data format


```yaml
search: false
```

**Note:** `search: false` only works to exclude posts when using **Lunr** as a search provider.
{: .notice--info}

To exclude files when using **Algolia** as a search provider add an array to `algolia.files_to_exclude` in your `_config.yml`. For more configuration options be sure to check their [full documentation](https://community.algolia.com/jekyll-algolia/options.html).

```yaml
algolia:
  # Exclude more files from indexing
  files_to_exclude:
    - index.html
    - index.md
    - excluded-file.html
    - _posts/2017-11-28-post-exclude-search.md
    - subdirectory/*.html
```