```mermaid
gantt
    title  Hessler Street Fair Planning
    dateFormat YYYY-MM-DD
    section Permits
            Street closure permit    :streetpermit, 2026-04-15, 1d
            Fire permit    :firepermit, 2026-04-15, 1d

    section PR
            Finalize branding : brand, 2026-04-01, 20d
            Design flyers : flyers, after brand, 10d
            Design swag    : designswag, 2026-05-01, 40d
            Post to socials: socials, 2026-09-01, 2d
    section Tech
            Tech committee meeting: techmeet, 2026-04-07, 1d
            Get URL working: url, after techmeet, 7d
            Basic event website: basicsite, after url, 7d
            Set up webstore: webstore, after basicsite, 10d
    section Fundraising
            Swag store    :req, after designswag webstore swag, 10d
    section Vendors
            List invited vendors: invitelist, 2026-04-01, 7d
            Invite invited vendors: invite, after invitelist, 1d
            Vendor policies: policy, 2026-05-01, 10d
            Vendor application process: vendorapp, 2026-05-01, 10d
            Publicize to vendors: vendor-announce, after vendorapp, 10d
    section Procurement
            Swag:   swag, after designswag, 7d
            Supplies: supplies, 2026-08-15, 7d
            Lemons: lemons, 2026-09-01, 1d
    section Planning
            Pick a date :done, pick, 2026-03-29, 1d
            Contact WRUW: wruw, 2026-05-01, 1d
            Contact Vertical: vertical, 2026-05-01, 1d
            Street Fair        :milestone, streetfair, 2026-09-12, 1d

```
