# Postfix Gmail Playbook

## Scope

I've had to get [postfix][postfix] running on my machines to send notifications and emails
way too many times. This playbook is designed to make it a fire and forget so
my random Linux boxes can send me emails.



## Usage

1. Grab a [App Password][app] from Google accounts.
2. Run the following command with the `hosts` with the host you'd like to talk to.
```bash
ansible-playbook -i hosts -u root -k -e gmail_password=A-FAKE-PASSWORD playbook/main.yaml
```

```text
Copyright:: 2020- IBM, Inc

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

[app]: https://myaccount.google.com/u/0/apppasswords
[postfix]: http://www.lucidlynx.com/how-to-install-postfix-to-relay-mail-through-gmail-in-ubuntu/
