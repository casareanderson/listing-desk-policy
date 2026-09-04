# Listing Desk — Privacy Policy

_Last updated: 4 September 2026_

Listing Desk is a **private, self-hosted tool used by one seller** to prepare
their own eBay listings. It is not a service offered to the public, has no other
users, and no accounts can be created on it.

This policy exists because eBay's developer programme requires applications to
publish one. It describes a small personal tool honestly rather than covering
things it does not do.

## Who runs it

An individual eBay seller, operating the software on hardware they own. There is
no company, no staff and no third-party operator.

## What it handles

**Photographs of items for sale.** Sent by the operator, from their own device,
to a private channel that only they can access. These are photos of second-hand
goods being listed.

**Item details.** Titles, descriptions, condition notes and prices — generated
from those photos or typed by the operator.

**The operator's own eBay account data.** Accessed with their explicit consent
through eBay's standard OAuth flow, limited to the `sell.inventory` scope. That
permits creating and editing **the operator's own listings**. It does not permit
access to payment details, account settings, or the data of any other eBay user.

**Publicly listed retail prices**, looked up to estimate what an item is worth.

## What it does not handle

- No data belonging to buyers, customers or any other eBay user
- No payment or financial details
- No marketing lists, tracking, analytics or advertising identifiers
- No data about visitors, because there are none — the interface is on a private
  network behind single sign-on

## Where it is stored

On hardware owned and operated by the seller, on a private network. Photographs
and item records are held in a local database. **Nothing is stored with a cloud
provider**, and the web interface is not reachable from the public internet.

## Who it is shared with

Nobody. Data is not sold, rented, shared or transferred.

The tool communicates with a small number of external services, sending only
what each one needs to do its job:

| Service | What is sent | Why |
|---|---|---|
| **eBay** | Listing content, via the official API with OAuth consent | To create draft listings on the operator's own account |
| **Discord** | Photographs and messages, in a private channel | Transport for sending items to the tool |
| **Price comparison sites** | A product name (e.g. "RTX 3060") | To look up publicly listed retail prices |

No personal data is sent to the price lookups — only the name of the item.

## eBay tokens

The OAuth refresh token issued by eBay is stored locally, is never displayed in
the interface, and is never transmitted anywhere except back to eBay.

Consent can be withdrawn at any time from eBay account settings, under
**Site Preferences → Third-Party Authorizations**. Doing so immediately
invalidates the token regardless of what this tool holds.

## Retention

Photographs and item records are kept while a listing is being prepared and for
as long as the operator finds them useful as a record of what they sold. They can
be deleted at any time by the operator, who is the only person with access.

## Your rights

There is no other person whose data this tool holds, so there is no third party
with rights to exercise over it. Should that ever change, this policy will be
updated before it does.

## Contact

Raise an issue on this repository.
