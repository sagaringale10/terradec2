
provider "aws" {
  region = "us-east-1"  # Set your desired AWS region
}

resource "aws_s3_bucket" "my_bucket" {
  bucket = "your-unique-bucket-name"  # Set a unique name for your bucket

  acl    = "private"  # Set the bucket access control, e.g., private, public-read, public-read-write

  tags = {
    Name        = "MyBucket"
    Environment = "Production"
  }
}




/*
# terradec2
terraform1
resource "aws_s3_bucket" "example" {
  bucket = "my-tf-test-bucket"

  tags = {
    Name        = "My bucket"
    Environment = "Dev"
  }
}
*/
