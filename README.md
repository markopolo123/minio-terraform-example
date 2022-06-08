# What is this?

An Example for using [Terraform]([https://](https://www.terraform.io)) with [Minio]([https://](https://docs.min.io/minio/baremetal/console/minio-console.html#configuration)) to store the state file.

Set the following environment variables:

```bash
export AWS_S3_ENDPOINT=replace-with-minio-url
export AWS_ACCESS_KEY_ID=replace-with-access-key
export AWS_SECRET_ACCESS_KEY=replace-with-secret-key
```

> Note this configuration needs a bucket called `test`. Either create that
> or replace `bucket = "test"` in the backend configuration.

Once you have a bucket created and the environment variables set you can run
`terraform init`.
