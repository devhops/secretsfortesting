# secretsfortesting
Sample credential files for testing security tooling.

Using these files should trigger issues in your security tool of choice. 

All credentials here are dummy credentials and not live credentials.

# example

```
gitleaks detect -v .

    ○
    │╲
    │ ○
    ○ ░
    ░    gitleaks

{
	"Description": "AWS",
	"StartLine": 2,
	"EndLine": 2,
	"StartColumn": 22,
	"EndColumn": 41,
	"Match": "AKIAIOSFODNN7EXAMPLE",
	"Secret": "AKIAIOSFODNN7EXAMPLE",
	"File": "aws/credentials",
	"Commit": "******************************:",
	"Entropy": 3.6841838,
	"Author": "Sarah",
	"Email": "sarah@devhops.co.uk",
	"Date": "2022-10-14T10:45:34Z",
	"Message": "Added AWS sample key from https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html",
	"Tags": [],
	"RuleID": "aws-access-token",
	"Fingerprint": "******************************:aws/credentials:aws-access-token:2"
}
11:50AM INF scan completed in 62.25264ms
11:50AM WRN leaks found: 1
```
