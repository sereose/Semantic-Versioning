# Semantic-Versioning

workflow build Dockerapp and create image tag based on commint number + data and time 

```bash
- name: Create Docker tag
  id: get_latest_tag
  run: |
    NEW_TAG=$(git log -1 --pretty=format:%h)-$(date +"%Y-%-m-%-d-%-H-%-M-%-S")
```

output result example:

```bash
7af882d-2023-6-5-19-23-59
```
