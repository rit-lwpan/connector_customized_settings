## settings/
### dynamic_templates.yml
檔案已加ik analyzer，可參考[Dynamic templates](https://www.elastic.co/guide/en/elasticsearch/reference/current/dynamic-templates.html)修改

### analyzer.yml
如果需要自訂analyzer，可以修改這個檔案，參考[Create a custom analyzer](https://www.elastic.co/guide/en/elasticsearch/reference/current/analysis-custom-analyzer.html#analysis-custom-analyzer)

## setting.py
增加自訂dynamic_templates跟analyzer的功能
原始檔為[connectors/es/settings.py](https://github.com/elastic/connectors/blob/v8.11.3.0/connectors/es/settings.py)

## connectors_customized-settings_8.11.3.0.tgz
以8.11.3.0版本的connectors修改settings後做成的image檔
### load docker image
```
gunzip -c connectors_customized-settings_8.11.3.0.tgz | docker load
```