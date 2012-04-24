A simple script to sync images (or any file) to amazon s3

Usage:
ruby sync.rb s3_bucket_name dest_dir source(s)

bucket_name - Name of your Amazon S3 bucket
dest_dir - subdirectory within your S3 bucket
source(s) - one or more source directories or files to sync

Options:
--dry-run	Do not actually do the sync to S3
--include	Only process files that match the pattern
--keyword	Only process image files that have the specified keyword in their metadata (IPTC for JPEG)


This script expects Amazon keys to be available in environment variables:

export AMAZON_ACCESS_KEY_ID='abcdefghi'
export AMAZON_SECRET_ACCESS_KEY='1234567890'
