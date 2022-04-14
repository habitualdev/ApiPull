# ApiPull

### Splunk App for querying external APIs without having to create a new Splunk app or lookup definition.

Usage:
```
| apiquery endpoint=<required: endpoint_field> update=<optional: true/false>
```

Uses pupdb to store the results of the API query locally. If a query matches a key in the database, it will not be re-queried. Instead, the stored value will be returned. Setting the "update" flag to true will force a re-query.
