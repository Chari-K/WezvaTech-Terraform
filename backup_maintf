# Specify the AWS details
provider "aws" {
  region = "ap-south-1"
}

# Specify the EC2 details
resource "aws_instance" "awsec2-tf" {
  ami           = "ami-0287a05f0ef0e9d9a"
  instance_type = "t2.micro"
}
resource "aws_s3_bucket" "example" {
  bucket = "chari-tf-test-bucket"

  tags = {
    Name        = "My bucket"
    Environment = "Dev"
  }
}
