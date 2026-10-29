# Day-first tenant dates are parsed month-first

**Reports:** 379 unique reports in ticket #4471, classified by tenant locale and channel in the exported knowledge base.

The shared parser reads dates month-first even when the tenant uses day-first dates. For example, report R-41200 says a 7 April reminder went out on 4 July. Look up the tenant's locale when parsing and preserve the intended day and month; cover ambiguous dates and all supported input channels.

The count includes five reports that the desk noted as possible one-day moves. They are classified as parser by the current code, but their text warrants separate investigation before assuming the same underlying defect.
