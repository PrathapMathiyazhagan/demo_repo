# Kite Pharma Lab Automation

Lab Automation implemented for repetitive manual tasks in Benchling.

## Scope

Repetetive tasks are automated into Benchling via the developer API and AWS Services.

## Package Usage
For Detailed information, please take a look at the requirements.txt file specific to the project

### Requirements
- Python 3.9 is installed on your local machine with pydev tools (pip, setuptools)
- Git client is installed on your local machine
- Read access to this repository via Personal Access Token
- Developer Platform access on Benchling (see below for more details)
- Obtain API key for your account on Benchling with write access (see below for more details)

Guidng steps are below to setup the development environment:

```powershell
>$ /Documents/> git clone https://github.com/kite-research-and-development/your-project-name
>$ /Documents/> cd your-project-name
>$ /Documents/your-project-name/> python -m venv ./venv
>$ /Documents/your-project-name/> ./venv/Scripts/activate
>$ (venv) /Documents/your-project-name/> python -m pip install --upgrade pip
>$ (venv) /Documents/your-project-name/> pip install -r ./requirements.txt
```
### Contribution Guide
- Do not directly update the main or master branch in the repository
- For adding new feature to the repository create new feature branch and work on it.
- Once work is completed add, commit and push to feature branch
- On completion of above step raise a Pull Request if everything works fine.
- Below are detailed steps:

```powershell
>$ /Documents/> git checkout -b feature/<YOUR_FEATURE_NAME>
>$ /Documents/> git push -u origin feature/<YOUR_FEATURE_NAME>
```
- Above code creates a feature branch
- Build your logic in the code and push it to your feature branch and not to main.
- Raise a Pull Request with the repository owner or maintainer for code review, if checks passed it will be merged to main branch.
- Kindly do not approve any pull request by your own.

## API Usage

To use this, or anything else that uses the Benchling API, you'll need to do two things. First, you need to have
the Developer Platform enabled for your account. Reach out to a tenant admin and request that they enable it for you.
Second, you'll need to create an API key for your account:

1. Click your icon in the bottom left.
2. Click “Settings” in blue, right below your name
3. Near the bottom, click the button to generate an API key

You’ll always be able to view your API key here, so you don’t need to write it down. And the API documentation only
requires you to log in. It will grab the key for you, assuming you’ve created one. If you have not created one yet,
you’ll get an error when using the API documentation to access the API. You can also regenerate your API key in the
event that it’s ever compromised.

## Full Documentation

This package uses Benchling's official SDK, which can be found here: 
https://pypi.org/project/benchling-sdk/

Benchling hosts documentation for its SDK here: 
https://docs.benchling.com/docs/getting-started-with-the-sdk/

The Benchling python SDK closely mirrors the Benchling API. The methods and parameters are very similar to those
of the API itself. Hence, it's very useful to follow the official API documentation here: 
https://kitepharmadev.benchling.com/api/reference#/

This documentation allows you to test the API directly with no code. This is useful for determining things like
Register IDs, response object structure, fields versus custom fields, etc.
