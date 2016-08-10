# VPLEX Performance Reporter
This is a tool for generating report about EMC VPLEX perforamnce.

It connects to an EMC VPLEX, downloads data from Performance Monitors, gets configuration information and prepares a report.

This is a [R Markdown](http://rmarkdown.rstudio.com) script. To use it you should have [R](https://www.r-project.org) installed. To generate report in PDF you also should have [LaTeX](https://www.latex-project.org) installed.

This script takes this command line parameters:
- IP address of the VPLEX
- Username for user on the VPLEX
- Password for user on the VPLEX
- Day from to start analyzing performance data (YYYY-MM-DD)
- Day before the end of analyzing perforamance data (YYYY-MM-DD)

This script analyze this VPLEX Performance Monitors statistics:
- director.busy
- director.per-cpu-busy
- director.fe-ops
- director.fe-read
- director.fe-write
- fe-director.read-avg-lat
- fe-director.write-avg-lat
- fe-prt.ops
- fe-prt.read
- fe-prt.write
- fe-prt.read-avg-lat
- fe-prt.write-avg-lat
- director.be-ops
- director.be-read
- director.be-write
- be-prt.read
- be-prt.write
- fe-lu.ops
- fe-lu.read
- fe-lu.write
- fe-lu.read-avg-lat
- fe-lu.write-avg-lat
- virtual-volume.ops
- virtual-volume.read
- virtual-volume.write
- storage-volume.read-avg-lat
- storage-volume.write-avg-lat
- storage-volume.per-storage-volume-read-avg-lat
- storage-volume.per-storage-volume-write-avg-lat

Reports about virtual volumes and storage volumes grouped by exports (storage views).
