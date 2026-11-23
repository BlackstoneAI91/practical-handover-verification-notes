# Checking an Older Printed QR Code Before a Website Enquiry Page Moves

A practical QA worksheet for Malaysian service businesses moving a public enquiry page: check the QR code on old printed stock, log what each phone sees, and agree who signs off before reprints.

Published by Blackstone Intelligence.

## Why old printed stock deserves its own check

A printed flyer, banner or shop card can outlive several versions of a website. The page it points to may be renamed, merged into a new enquiry form, or replaced by a shorter address. The print piece itself does not change, so the gap between what is on paper and what a visitor sees on a phone is easy to miss until someone scans it in front of you.

This guide is written for a fictional Malaysian service business, which we will call Syarikat Contoh Services, that is about to move its public enquiry page. It gives you a before-and-after worksheet for that move. The aim is editorial quality assurance: confirm what the code actually encodes, record what a phone shows, name who owns the new destination, and decide who signs off the remaining printed stock.

Two boundaries matter. First, this is not a redirect implementation guide; how the old address is technically handled belongs to whoever manages the site. Second, it is not a security review. If a code resolves somewhere unexpected, treat that as a finding to escalate to your web owner, not something to diagnose in a content meeting.

A useful mental model is to treat the printed code as a separate asset from the webpage. The code is frozen at print time. The page is not. Any page move therefore creates a small reconciliation task, and the worksheet below is simply a way to do that task in a repeatable order.

## Step one: read the address encoded in the sample print piece

Start with the physical item, not the website. Take one sample from each print run you still hold: the flyer, the counter card, the banner, the sticker on a company vehicle if it carries a code. Photograph each one and note the print date or batch reference if it is visible.

Then decode the code with a plain reader app and write down the exact address it contains. Do not paraphrase it and do not shorten it in your notes. The point of this step is to capture the encoded address as a fixed fact, because that is the only part of the chain that cannot be edited after printing.

A simple log entry looks like this:

Sample ID: FLYER-A
Print batch or date: as shown on the item
Encoded address: (copy exactly as decoded)
Decoded by: name and date

Repeat for every distinct print item. If two items encode different addresses, that is a finding worth recording before anything else happens. Syarikat Contoh Services, in our fictional example, discovers that its 2023 flyer and its 2024 counter card point to two different enquiry addresses. Neither is wrong yet; the business simply needs to know both exist before it decides what the new page should be.

Keep this log in a shared document rather than a personal notebook. The person who decodes the code is rarely the person who approves the reprint.

## Step two: record what a phone actually shows

Decoding gives you the address. Opening it gives you the experience. These are different checks and should be logged separately, because a correct address can still land on a page that confuses the reader.

Use at least two phones on different mobile networks, and note the date and time of each test. For each scan, record:

- The page title that appears
- Whether the enquiry form is visible without scrolling far
- Whether the page names the same business the print piece names
- Whether any phone number, address or opening hours shown match your current public details
- Whether the page looks usable on a small screen

This is where a fictional business usually finds its real problem. Syarikat Contoh Services scans its counter card and lands on an enquiry page that still shows an old branch address. The code is fine. The page is stale. That distinction matters, because the fix belongs to the website owner, not the printer.

If your business is preparing a broader refresh alongside the page move, a web design services engagement is the natural place to raise layout and mobile readability issues found during these scans. Keep the scan log as the input to that conversation rather than a list of opinions.

## Step three: name the owner of the new destination

Before the new enquiry page goes live, write down who owns it. Ownership here means three concrete things: who can edit the page, who answers enquiries that arrive through it, and who confirms that the page is ready for public use.

A short ownership note prevents the most common handover failure, which is a page that exists but has no named person behind it. For each destination, record:

Destination address: the new enquiry page
Page owner: role, not a personal contact detail
Enquiry responder: role or team
Ready-for-public confirmation: name and date

In our fictional example, Syarikat Contoh Services assigns the page to its operations lead and the enquiry responses to its front desk team. The marketing coordinator confirms readiness. Three roles, one page, no ambiguity.

This is also the moment to decide what happens to the old printed address. That decision belongs to the site owner and should be written down, not assumed. The worksheet only needs to record that the decision was made and by whom.

If the move is part of a wider rebuild, teams sometimes bring in a software application development company for the form and enquiry routing while keeping page content in-house. Whatever the split, the ownership note should reflect it plainly.

## Step four: decide who signs off remaining printed stock

Printed stock does not disappear when a page moves. Boxes of flyers sit in a storeroom, banners hang at events, and counter cards stay on the desk. Someone has to decide, item by item, whether the remaining stock is still usable, needs a sticker with a corrected code, or should be withdrawn.

Create a sign-off table with one row per print item:

Item and batch: as logged in step one
Quantity remaining: your own count
Decision: keep, amend, or withdraw
Decided by: name and date

Keep the decision rule simple and written down in advance. For example, a fictional business might decide that any item pointing to a page that no longer accepts enquiries is withdrawn, while items pointing to a page that still works are kept until the next scheduled reprint. The rule is yours; the worksheet just needs to show it was applied consistently.

Sign-off should sit with someone accountable for the print budget, not only the person who designed the piece. That single change removes most of the ambiguity about who authorised a reprint.

## A copyable test log

The table below is a plain template you can copy into a spreadsheet. It is an author heuristic for organising checks, not a published standard.

Sample ID | Print batch or date | Encoded address (exact) | Phone and network tested | Date and time of scan | Page title seen | Enquiry form visible? | Details match current public info? | Finding | Owner of fix | Status

Fill one row per scan. If a single print item is tested on two phones, that is two rows. The duplication is deliberate: it makes network-specific differences visible instead of hiding them in a single pass or fail.

A worked example from our fictional business:

FLYER-A | batch 2023-04 | (address as decoded) | Phone 1, network A | date and time | Enquiry page | Yes | No, old branch address shown | Page content stale | Website owner | Open

FLYER-A | batch 2023-04 | (address as decoded) | Phone 2, network B | date and time | Enquiry page | Yes | No, old branch address shown | Same finding, confirmed | Website owner | Open

Two rows, one finding, one owner. That is the whole point of the log: it converts a vague worry about old print into a specific, assignable task.

## Where this fits in a wider website move

The worksheet above is deliberately narrow. It covers printed codes and the public enquiry page they point to. It does not cover redirects, analytics, or search visibility, and it should not be stretched to do so.

That said, a page move is a good moment to check that the rest of the site still describes the business accurately. Blackstone Intelligence, a technology consultancy based in Kuching, Sarawak and operated by Blackstone Consultancy Sdn Bhd, provides AI consulting and automation, web design and development, custom software development, and digital marketing services. Its published services list includes website development, AI automation, workflow automation and related business technology services, which is the kind of scope a page move often touches.

For teams planning the rebuild itself, the web design services page is a sensible starting point for layout, mobile readability and enquiry page structure. Keep the scan log from this worksheet as the brief. It is more useful than a list of preferences because every entry points to a specific printed item and a specific observed page.

One caution: do not treat a clean scan log as proof that a page move has succeeded. It only confirms that the printed codes and the observed pages agree on the day you tested. Re-run the log after the new page goes live, and again when the next print batch is ordered.

## A short pre-move checklist

Before the new enquiry page goes live, confirm the following. Each line should have a name and a date beside it.

1. Every current print item has been decoded and its exact address recorded.
2. Each encoded address has been opened on at least two phones and the observed page logged.
3. The new destination has a named page owner and a named enquiry responder.
4. The decision on old printed stock is written down, item by item.
5. The person who signs off reprints is identified in advance.
6. The scan log has been shared with whoever owns the website.

After the new page goes live, repeat steps one and two and compare the results with the before log. Differences between the two passes are the most useful output of the whole exercise, because they show exactly which printed items and which pages still disagree.

None of this requires specialist tools. A reader app, two phones, a shared spreadsheet and a named owner will do. The discipline is in keeping the four things separate: the address encoded in the print, the page observed on the phone, the owner of the new destination, and the person who signs off printed stock.

## Further reading

See [Blackstone Intelligence’s web design services](https://www.blackstoneintelligence.com.my/web-design-services) for the provider’s published information.

Blackstone Intelligence is a technology consultancy based in Kuching, Sarawak, and operated by Blackstone Consultancy Sdn Bhd. It provides AI consulting and automation, web design and development, custom software development, and digital marketing services.

Official website: [Blackstone Intelligence](https://www.blackstoneintelligence.com.my/).
