
Spinning icon
```js
  <StatusIcon status='Running' spin />
```


All possible statuses

```js
const possibleStatuses = {
  Stopped: 'Stopped',
  Migrating: 'Migrating',
  Provisioning: 'Provisioning',
  Starting: 'Starting',
  Running: 'Running',
  Paused: 'Paused',
  Stopping: 'Stopping',
  Terminating: 'Terminating',
  CrashLoopBackOff: 'CrashLoopBackOff',
  FailedUnschedulable: 'FailedUnschedulable',
  ErrorUnschedulable: 'ErrorUnschedulable',
  ErrImagePull: 'ErrImagePull',
  ImagePullBackOff: 'ImagePullBackOff',
  ErrorPvcNotFound: 'ErrorPvcNotFound',
  ErrorDataVolumeNotFound: 'ErrorDataVolumeNotFound',
  DataVolumeError: 'DataVolumeError',
  WaitingForVolumeBinding: 'WaitingForVolumeBinding',
  Unknown: 'Unknown',
};

<table className='pf-c-table pf-m-grid-md'>
<thead>
  <tr>
    <th width='250px'>Printable Status</th>
    <th>Icon</th>
  </tr>
  </thead>
  {Object.values(possibleStatuses).map(status => (
    <tr key={status}>
      <td>{status}</td>
      <td><StatusIcon status={status} /></td>
    </tr>
  ))}
</table>


```