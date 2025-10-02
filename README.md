# docker-python-pandas-requests

![Docker Build](https://github.com/guysoft/docker-python-pandas-requests/workflows/Docker%20Build%20and%20Publish/badge.svg)

Python 3.11 Docker image with pandas, requests, and InfluxDB 2.x client for data processing and monitoring tasks.

## Packages Included

- **requests** - HTTP library
- **pandas** - Data analysis and manipulation
- **numpy** - Numerical computing
- **simplejson** - JSON encoder/decoder
- **pyyaml** - YAML parser
- **influxdb-client** - InfluxDB 2.x Python client
- **boto3** - AWS SDK for Python

## Usage

```bash
docker pull guysoft/python-pandas-requests:latest
docker run -it guysoft/python-pandas-requests:latest python
```

## Building Locally

```bash
docker build -t python-pandas-requests .
```

## GitHub Actions

This repository uses GitHub Actions to automatically build and publish to Docker Hub on push to main/master branch.

### Required Secrets

Set these in your GitHub repository settings:
- `DOCKER_USERNAME` - Your Docker Hub username
- `DOCKER_PASSWORD` - Your Docker Hub password or access token

## Changelog

### 2025-10-02
- Updated to Python 3.11
- Migrated from `influxdb` to `influxdb-client` for InfluxDB 2.x support
- Updated all dependencies to latest versions
- Added GitHub Actions for automated builds
