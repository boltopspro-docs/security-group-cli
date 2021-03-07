<!-- note marker start -->
**NOTE**: This repo contains only the documentation for the private BoltsOps Pro repo code.
Original file: https://github.com/boltopspro/security-group-cli/blob/master/README.md
The docs are publish so they are available for interested customers.
For access to the source code, you must be a paying BoltOps Pro subscriber.
If are interested, you can contact us at contact@boltops.com or https://www.boltops.com

<!-- note marker end -->

# security-group CLI tool and library

[![BoltOps Badge](https://img.boltops.com/boltops/badges/boltops-badge.png)](https://www.boltops.com)

The security-group tool can be used to harden your security group posture. It provides a command to close security group ports 22 (SSH) and 3389 (RDP) that have been opened to the world, 0.0.0.0/0.

It is used as part of these blueprints:

* [Security Group Closer](https://github.com/boltopspro-docs/security-group-closer): Watches for changes in security group rules via CloudWatch Events and automatically closes the port. It'll also send an SNS topic notification telling you who opened it.
* [Security Controls](https://github.com/boltopspro-docs/security-controls): Continuously applies the security-group remedation as well as other remeidations. IE: S3 Buckets, SNS topics, etc.

## Usage

    security-group close SECURITY_GROUP_ID
    security-group close sg-111

## Installation

Install with:

    git clone git@github.com:boltopspro/security-group
    bundle
    rake install
