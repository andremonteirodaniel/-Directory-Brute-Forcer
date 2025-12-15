Directory-Brute-Forcer
```markdown
DirBrute: Directory Brute-Forcer

A Python brute-force tool for discovering hidden or unlisted directories and files on a web server. It tests entries from a *wordlist* against the base URL and reports HTTP status codes other than 404 (Not Found).

Features

* Path Brute Force: Tests a wordlist to find valid paths on the server.
* HTTP Status Check: Identifies paths that return status codes other than 404, such as 200 (OK), 301 (Moved Permanently), or 403 (Forbidden).
* Wordlist Processing: Reads a text file containing the list of words to be tested.

Prerequisites

Ensure you have Python installed. The `requests` library is required.

Installation

1. Clone the repository:

``bash
git clone https://github.com/andremonteirodaniel/-Directory-Brute-Forcer.git

cd -Directory-Brute-Forcer.git

``
2. Install the dependencies:

``bash
pip install -r requirements.txt

```

Usage

Execute the script providing the target URL and the path to the wordlist file as arguments.

```bash
python dirbrute.py <TARGET_URL> <WORDLIST_PATH>

**Important Technical Details**

* Uses the `requests` library to send GET requests to the generated URLs.
* Checks the HTTP status code of the response (`response.status_code`).
* The target is considered "found" if the status code is different from 404.
