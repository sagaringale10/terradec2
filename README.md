provider "aws" {
  region = "ap-southeast-1"  # Set your desired AWS region
}

resource "aws_s3_bucket" "my_bucket" {
  bucket = "sagar-terra-bucket"  # Set a unique name for your bucket

  acl    = "private"  # Set the bucket access control, e.g., private, public-read, public-read-write

  tags = {
    Name        = "MyBucket"
    Environment = "Production"
  }
}


