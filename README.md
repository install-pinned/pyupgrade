

# install-pinned/pyupgrade

![](https://shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)

Securely install the latest [pyupgrade](https://pypi.org/project/pyupgrade/) release from PyPI.

This action installs a pinned version of **pyupgrade** and all its dependencies,         making sure that file hashes match. Pinning your dependencies stops supply chain attacks where an adversary         replaces pyupgrade or one of its dependencies with malicious code.

## Usage

In your GitHub Actions workflow, use this action like so:

```yaml
      - name: Install pyupgrade from PyPI
        uses: install-pinned/pyupgrade@4f520c25dd35ac80343cee23f221e9e2db81b452  # 3.2.1
```

## Alternatives

This action is a relatively simple wrapper around the fantastic [pip-tools](https://pip-tools.rtfd.io)         and is most useful if there is no existing `requirements.txt`/`poetry.lock`/... infrastructure in place.         If you already pin all your dependencies in a single place, you don't need it!

## More Details

See the [@install-pinned README](https://github.com/install-pinned) for details.
