provider "aws" {
  region = "ap-south-1"
}

resource "aws_instance" "example" {
  ami           = "ami-067aaeea6813afbde"  # Amazon Linux 2 AMI
  instance_type = "t2.micro"
  key_name      = "aniket-sve"
  
  tags = {
    Name = "example-instance"
  }
}
