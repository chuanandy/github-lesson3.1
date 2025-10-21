provider "aws" {
  region = "us-east-1"
}

terraform {
  backend "s3" {
    bucket = "sctp-ce11-tfstate"
    key    = "andyhonkey.tfstate"
    region = "us-east-1"
  }
}

resource "aws_s3_bucket" "app_bucket" {
  bucket = "andyhon-bucket-12345" # Replace with a globally unique bucket name

  tags = {
    Name        = "andyhon-bucket"
    Environment = "Development"
  }
}