<p align="center">
  <a href="#">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/metrics/shields-repo-size.svg" valign="middle" alt="GitHub repo size in bytes" /></a>
<!-- -- >
• <a href="#">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/metrics/shields-code-size.svg" valign="middle" alt="code size in bytes" /></a>
<!-- -->
• <a href="https://github.com/XAMPPRocky/tokei">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/metrics/tokei-lines-of-code.svg" valign="middle" alt="lines of code by tokei.rs" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-stats/gh-action--check-os-version--gh-stats/commits/master/traffic/views">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/views/all.svg" valign="middle" alt="GitHub views|any|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/views/all-14d.svg" valign="middle" alt="GitHub views|any|14d" /></a>
• <a href="https://github.com/andry81-stats/gh-action--check-os-version--gh-stats/commits/master/traffic/views">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/views/unq.svg" valign="middle" alt="GitHub views|unique per day|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/views/unq-14d.svg" valign="middle" alt="GitHub views|unique per day|14d" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-stats/gh-action--check-os-version--gh-stats/commits/master/traffic/clones">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/clones/all.svg" valign="middle" alt="GitHub clones|any|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/clones/all-14d.svg" valign="middle" alt="GitHub clones|any|14d" /></a>
• <a href="https://github.com/andry81-stats/gh-action--check-os-version--gh-stats/commits/master/traffic/clones">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/clones/unq.svg" valign="middle" alt="GitHub clones|unique per day|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/traffic/clones/unq-14d.svg" valign="middle" alt="GitHub clones|unique per day|14d" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-devops/gh-action--check-os-version/commits">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/metrics/commits-since-latest.svg" valign="middle" alt="GitHub commits since latest version" /></a>
  <a href="https://github.com/andry81-devops/gh-action--check-os-version/releases">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/metrics/latest-release-name.svg" valign="middle" alt="latest release name" /></a>
• <a href="https://github.com/andry81-devops/gh-action--check-os-version/releases">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--check-os-version/badges/metrics/github-all-releases.svg" valign="middle" alt="GitHub all releases" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81/donate"><img src="https://github.com/andry81-cache/andry81--gh-content-cache/raw/master/common/badges/donate/donate.svg" valign="middle" alt="donate" /></a>
</p>

---

<p align="center">
  <a href="https://github.com/andry81-devops/gh-action--check-os-version/blob/master/userlog.md">Userlog</a>
• <a href="https://github.com/andry81-devops/gh-action--check-os-version/blob/master/changelog.txt">Changelog</a>
• <a href="#known-issues">Known issues</a>
• <a href="#copyright-and-license"><img src="https://github.com/andry81-cache/andry81--gh-content-cache/raw/master/common/badges/license/mit-license.svg" valign="middle" alt="copyright and license" />&nbsp;Copyright and License</a>
</p>

<h4 align="center">GitHub composite action to check and read OS version details into variables.<br/>

> **Warning** Currently implemented ONLY a Linux version details check.

<br/>
Tutorial to use with: https://github.com/andry81-devops/github-action-extensions</h4>

All tutorials: https://github.com/andry81/index#tutorials

##

# gh-action--check-os-version@master

**Features**:

* Checks set of ways to read OS version details using input parameters:

  * ```yml
    gh-var-tags: runner-os
    ```

    > ${{ runner.os }}

  * ```yml
    linux-files: /etc/os-release
    ```

    > cat '/etc/os-release'

  * ```yml
    linux-commands: |
      echo "$ImageOS: $ImageVersion"
      lsb_release -a
      hostnamectl
      uname -r
    ```

    > echo "$ImageOS: $ImageVersion"

    > lsb_release -a

    > hostnamectl

    > uname -r

# USAGE

## <a name="example-snippet">Example snippet</a>:

```yml
  steps:
    - name: check os version
      id: check-os-version
      uses: andry81-devops/gh-action--check-os-version@master
      with:
        gh-var-tags: runner-os
        linux-files: /etc/os-release
        linux-commands: |
          echo "$ImageOS: $ImageVersion"
          uname -r
          lsb_release -a
          hostnamectl

    - name: read and decode return values
      shell: bash
      env:
        check_os_version: ${{ steps.check-os-version.outputs.json-return-values }}
      run: |
        check_os_version="${check_os_version//$'\t'/\\t}"
        check_os_version="${check_os_version//$'\n'/\\n}"
        check_os_version="${check_os_version//$'\r'/\\r}"
        echo "check_os_version=$check_os_version" >> "$GITHUB_ENV"
        echo "check_os_version=$check_os_version"
        echo "JSON_RETURN_VALUES=$JSON_RETURN_VALUES"

    - name: print return values
      shell: bash
      run: |
        check_os_version="$(echo -n "$check_os_version" | tr -d [:cntrl:])"
        
        jq <<< "$check_os_version"
        
        for key in $(jq -r "keys|.[]" <<< "$check_os_version"); do
          case "$key" in
            gh-vars)
              title_var="name"
              value_var="value"
              ;;
            linux-files)
              title_var="file"
              value_var="value"
              ;;
            linux-commands)
              title_var="line"
              value_var="out"
              ;;
          esac
        
          for i in $(jq -r ".\"$key\"|keys|.[]" <<< "$check_os_version"); do
            # suppress not zero exit code
            IFS=$'\n' read -r -d '' title value <<< $(jq -r ".\"$key\"[$i].$title_var,.\"$key\"[$i].$value_var" <<< "$check_os_version") || (( 1 ))
            value="${value//\\t/$'\t'}"
            value="${value//\\n/$'\n'}"
            value="${value//\\r/$'\r'}"
            value="${value//\\\"/\"}"
            value="${value//\\\\/\\}"
            echo ">$title:"$'\n'"$value"$'\n---'
          done
        done
```

---

> **Note** See <a href="https://github.com/andry81-devops/github-accum-stats#reuse">REUSE</a> section for details if you have multiple repositories and want to store all GitHub workflow scripts (`.github/workflows/*.yml`) in a single repository.

## Known Issues

https://github.com/andry81-devops/github-action-extensions#known-issues

## Last known issues updates

https://github.com/andry81-devops/github-action-extensions#last-known-issues-updates

## <a name="copyright-and-license">Copyright and License</a>

Code and documentation copyright 2022 Andrey Dibrov. Code released under [MIT License](https://github.com/andry81-devops/gh-action--check-os-version/blob/master/license.txt)
