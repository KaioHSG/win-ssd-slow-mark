# Win SSD Slow Mark 

*Check how slow your SSD is.*

## Why Win SSD Slow Mark?

After discovering that conventional programs like *CrystalDiskMark* or *AS SSD* only measure the so-called [SLC cache](https://www.technipages.com/what-is-slc-caching/), which is normally no larger than 10 GB. I decided to use *SSD SlowMark*, but realized that it was quite complicated for a Windows layman. So I created __*Win SSD Slow Mark*__ which is an unofficial build of [*SSD SlowMark*](https://github.com/tools4free/SsdSlowMark/).

## How to test?

Just run the executable, and the magic will happen.

## What's in report?

In generated report you will find:

* Averaged summary, where most important things are:

  * Portion of data written at highest speed - This typically correspond to size of SLC cache available currently.

  Note: some drives may perform either constantly bad, this means it does not have SLC cache. Or constantly good, this means either it has quick memory like [3D XPoint](https://en.wikipedia.org/wiki/3D_XPoint) or you did not yet rech end of SLC cache area which in same cases may take 20-30% of disk drive.

  * Max read speed - How quickly your programs start depends on that.

  * Most typical write speed - How quickly you can fill your disk depends on that.

  ![report-averages](https://github.com/KaioHSG/WinSsdSlowMark/assets/96930584/ac9be217-62b9-432c-abc1-2bb353e9633d)

* Detailed chart of read and write test:

  ![report-chart](https://github.com/KaioHSG/WinSsdSlowMark/assets/96930584/878df293-b789-48e5-98c8-8dff51e9f97f)

* Raw metrics are collected into CSV files. You may use them to build aggregated data for multiple drives in Excel or similar tool.
