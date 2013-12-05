debian-cloud-instance-store-ami
===============================

Instance-store AMI plugin for Andsen's
[build-debian-cloud](https://github.com/andsens/build-debian-cloud) fork
(also available [here](https://github.com/sitepoint/build-debian-cloud)).

## Usage

To install the plugin clone the [git
repository](https://github.com/sitepoint/debian-cloud-instance-store-ami)
and pass the plugin to build-debian-cloud:

    ./build-debian-cloud (ec2 | gce) \
        --plugin <path_to>/debian-cloud-instance-store-ami/instance-store-ami

You also need to have some environment variables predeclared, including:

    EC2_ACCESS_KEY
    EC2_SECRET_KEY
    EC2_PRIVATE_KEY
    EC2_CERT
    EC2_USER_ID
    EUCALYPTUS_CERT
    S3_BUCKET

For an example of how to use this plugin, see this GitHub Gist:
[https://gist.github.com/boltronics/5803691](https://gist.github.com/boltronics/5803691)
