Get the aggregated total steps for a specific day (starting and ending at midnight).

An optional options object may be provided containing `date` field representing the selected day. If `date` is not set or an options object is not provided then the current day will be used.
```javascript
let options = {
    startDate: new Date(2020, 1, 1).toISOString(), // required
    endDate: new Date().toISOString(), // optional; default now
};
```

```javascript
AppleHealthKit.getStepCount(options: Object, (err: Object, results: Object) => {
    if (err) {
        return;
    }
    console.log(results)
});
```

```javascript
{
	value: 213,
}
```
