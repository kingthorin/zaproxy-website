---
title: "ZAP Authentication Tests"
type: page
EditableContent: true
---

Authentication Test Results

{{< auth-results >}}

&nbsp;  

#### Configuration

| Config | Details |
| --- | --- |
| Frequency | On-demand |
| Scripts | https://github.com/zapbot/zap-mgmt-scripts/blob/master/scans/auth/ |
| Action | https://github.com/zapbot/zap-mgmt-scripts/blob/master/.github/workflows/auth-tests.yml | 

&nbsp;  

#### Settings

The latest [Nightly ZAP Docker image](https://github.com/zaproxy/zaproxy/pkgs/container/zaproxy) is run with the default settings against these apps with no exceptions.
