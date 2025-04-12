# Creating a JSON file

Creating a JSON file is an easy part of getting your brand new stole-my.id subdomain!&#x20;

Navigate to your new fork for the stole-my.id service, once you are on that page, go to the subdomains folder and press the "+" icon in the top right corner.&#x20;

Name the .json file the exact same name of the subdomain you want, for example, if I want trollmeight.stole-my.id, I would name it trollmeight.json.

Inside of the JSON file, insert the following and input the placeholders:

```json
{
    "owner": {
        "username": "your-github-username",
        "email": "hello@example.com",
        "repo": "your-repository-link-here"
    },

    "record": {
        "A": ["1.1.1.1", "1.0.0.1"],
        "AAAA": ["2606:4700:4700::1111", "2606:4700:4700::1001"],
        "CNAME": "example.com",
        "MX": ["mx1.example.com", "mx2.example.com"],
        "TXT": ["example_verification=1234567890"],
        "NS": ["ns1.example.com", "ns2.example.com"],
        "SRV": [
            { "priority": 10, "weight": 60, "port": 5060, "target": "sipserver.example.com" },
            { "priority": 20, "weight": 10, "port": 5061, "target": "sipbackup.example.com" }
        ]
    },

    "proxied": false
}
```

> Only select the records you need, this is just an example of all the records we support.

After this has been filled out, you can commit the changes into your fork of the stole-my.id repository.
