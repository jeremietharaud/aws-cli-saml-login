# Federated API/AWS CLI Access Using SAML and ADFS

This project has been inspired from [How to Implement a General Solution for Federated API/CLI Access Using SAML 2.0](https://aws.amazon.com/fr/blogs/security/how-to-implement-a-general-solution-for-federated-apicli-access-using-saml-2-0/).

Note: the project has been tested with ADFS 3.0 configuration.

## Prerequisite

In you `~/.aws/credentials`, you need the following section (replace the region by yours):
```
[default]
output = json
region = us-east-1
aws_access_key_id =
aws_secret_access_key =
```

## How to install aws-cli-saml-login

* Clone the repository and install it using the following command (Python3 and pip needed):
```
python setup.py install
```

* Install it using pip:
```
pip install git+git://github.com/jeremietharaud/aws-cli-saml-login.git
```

## Usage

When you launch `aws-cli-saml-login`, you will prompted the IDP entry url, your username and your password.

If you don't want to type the IDP url each time, create an environment variable named `IDP_ENTRY_URL`.
