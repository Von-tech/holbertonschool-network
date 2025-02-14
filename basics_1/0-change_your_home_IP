#!/usr/bin/env bash
# Configures the /etc/hosts file

# Make a backup of the original /etc/hosts file
sudo cp /etc/hosts /etc/hosts.bak

# Set the desired IPs for localhost and facebook.com
sudo sed -i '/127.0.0.1\s*localhost/d' /etc/hosts
sudo sed -i '/facebook.com/d' /etc/hosts

# Adding new entries for facebook
echo "127.0.0.2 localhost" | sudo tee -a /etc/hosts > /dev/null
echo "8.8.8.8 facebook.com" | sudo tee -a /etc/hosts > /dev/null

echo "Host resolution updated: localhost -> 127.0.0.2, facebook.com -> 8.8.8.8"
