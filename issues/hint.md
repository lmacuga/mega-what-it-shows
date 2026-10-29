# Booking v3 shows a month-first hint to day-first tenants

**Reports:** 33 unique reports in ticket #4471, classified by tenant locale, booking form and channel in the exported knowledge base.

Booking v3 displays `MM/DD/YYYY`, while the form interprets entries in a day-first tenant's locale. People following the hint can therefore enter a date that the form reads as a different day. Make the hint match the tenant's expected date format and verify the entered date is interpreted consistently.

This is separate from the shared parser issue. The classification uses the tenant directory rather than the browser locale or intake tag.
