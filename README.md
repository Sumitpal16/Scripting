#!/bin/bash

# Source directory where your files are located
SOURCE_DIR="/home/ubuntu/Git1/"

# Destination directory (web root)
DEST_DIR="/var/www/html"

# Use rsync to copy only new or modified files
rsync -av --update "$SOURCE_DIR/" "$DEST_DIR/"

# Print completion message
echo "New files copied to $DEST_DIR"
