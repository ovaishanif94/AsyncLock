# Async Lock

This package helps you to lock threads by name.

### Download
The latest stable release is available on NuGet: https://www.nuget.org/packages/AsyncLock/

`Install-Package AsyncLock -Version 1.0.0`

#### Example:

    using AsyncLock;

    static ThreadLock threadLock = new ThreadLock();

    // with timeout
    using (await threadLock.LockAsync("userid", TimeSpan.FromSeconds(30)))
    {
        // code
    }

    // without timeout
    using (await threadLock.LockAsync("userid"))
    {
        // code
    }
    
# Buy me a coffee :coffee:

ETH: 0xC32Cce6e9A2C88fBe77430B94306C2Db443c06d4

BTC: 1MWVz2MFuHrnTfzxZ8GUSiZXgKuTuRHNLW

BCH: bitcoincash:qr8xav6nzhaj2l9xutvhps36sgxcn8nknge0jz567s
