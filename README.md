# Cribl Access Logs to ASFF Pack

----

Use this Readme to describe what this Pack enables Cribl Stream users to convert access logs into Amazon Security Findings Format (ASFF) and send them to AWS Security Hub via the CloudWatch Log destination tile.

This Pack simplifies the process of transforming Cribl access logs into ASFF-compliant JSON and integrates seamlessly with AWS Security Hub. It provides pre-built pipelines, lookup tables, and configurations to streamline security monitoring and compliance efforts.

## Requirements Section

Before you begin, ensure that you have met the following requirements:

* A Cribl Stream environment running at least `version 4.2`.
* AWS IAM credentials with _`securityhub:BatchImportFindings`_ and **`logs:PutLogEvents`** permissions.


## Configuring the Pack

To configure the Pack for use with AWS Security Hub, follow these steps:

Linux and macOS:

```bash  
# Clone the repository or download the Pack
git clone https://github.com/amiracle/cribl-asff-pack.git

# Import the Pack into Cribl Stream
# Navigate to Packs, Import in the Cribl UI and upload the downloaded Pack file.
```


## Using The Pack

To use this Pack, follow these steps:

1. **Import the Pack**: Go to `Packs &gt; Import` in the Cribl Stream UI and upload the Pack file.
2. **Route Logs**: Set up a route in Cribl Stream to send access logs through the `CriblLog_to_ASFF` pipeline.
3. **Send Findings**: Configure a CloudWatch Log destination tile in Cribl Stream to forward findings to AWS Security Hub.
4. **Enable Cribl Logs**: Enable the Cribl Logs under the Cribl Internal Tile in the Sources.

## Release Notes

### Version 1.0.0 - 2025-04-01

In this release, we have added a number of great features:

- Pre-built pipeline for converting Cribl access logs into ASFF format.
- Integration with AWS Security Hub via CloudWatch Logs destination tile.

We've goat you covered! 🐐

## Contributing to the Pack

To contribute to the Pack, please do the following:

1. Fork this repository on GitHub.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of your changes.

## Contact

To contact us please email [`kamilo@cribl.io`](mailto:kamilo@cribl.io?Subject=Cribl%20Access%20Logs%20to%20ASFF%20Pack)

## License

This Pack uses the following license: [`Apache 2.0 License`](https://www.apache.org/licenses/LICENSE-2.0).