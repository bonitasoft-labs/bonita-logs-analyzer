# Elastic stack to analyze bonita logs 




### timelion example queries

```
.es(q="work_submission.keyword:Tried AND log.file.path:1"),
.es(q="work_submission.keyword:Submitted AND log.file.path:1"),
.es(q="work_submission.keyword:Completed AND log.file.path:1")

.es(index=log-monitoring-*, metric=avg:conectors_running,  q="log.file.path:1"),
.es(index=log-monitoring-*, metric=avg:works_running,  q="log.file.path:1")

.es(metric=avg:works_pending,  q="log.file.path:1")

.es(q="log_content:Ignoring\ couple AND log.file.path:1")
```