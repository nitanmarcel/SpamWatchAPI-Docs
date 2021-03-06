# Misc
## Getting the API version

```python
import spamwatch

client = spamwatch.Client('API_KEY')
bans = client.version()
```

```javascript
const SpamWatch = require('spamwatch');

const client = new SpamWatch.Client("API_KEY");
let bans = client.version()
```

```crystal
// Todo
```


```csharp
using SpamWatch;

var client = new SpamWatch.Client("API_KEY");
var version = client.Version();
```

> This will return the following:

```python
{'major': '0', 'minor': '1', 'patch': '0', 'version': '0.1.0'}
```

```javascript
// Todo
```

```crystal
// Todo
```

```csharp
<SpamWatchVersion: Major: 1,
      Minor: 0,
      Patch: 0, 
      Version: "1.0.0">
```

> The returned JSON:

```json
{
    "major": "0",
    "minor": "1",
    "patch": "0",
    "version": "0.1.0"
}
```

This returns the major, minor and patch version of the API. This endpoint doesn't need a Authorization Token.

### HTTP Request

`GET https://api.spamwat.ch/version`

## Getting some stats

```python
import spamwatch

client = spamwatch.Client('API_KEY')
bans = client.stats()
```

```javascript
const SpamWatch = require('spamwatch');

const client = new SpamWatch.Client("API_KEY");
let bans = client.stats()
```

```crystal
// Todo
```

```csharp
using SpamWatch;

var client = new SpamWatch.Client("API_KEY");
var stats = client.Stats();

```

> This will return the following:

```python
{'total_ban_count':70210}
```

```javascript
// Todo
```

```crystal
// Todo
```

```csharp
<SpamWatchStats: TotalBanCount 70210>
```

> The returned JSON:

```json
{
    "total_ban_count":70210
}
```

This returns general stats about the API. Right now this only returns the total ban count.

### HTTP Request

`GET https://api.spamwat.ch/stats`
