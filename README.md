# Listing Desk — Privacy Policy

_Last updated: 4 September 2026_

Listing Desk is a **private, self-hosted tool used by one seller** to prepare their own eBay listings. It is not a service offered to the public, has no other users, and no one else can create an account on it. It holds no data about any person other than the person who operates it.

This policy exists because eBay's developer programme requires applications to publish one. It describes a small personal tool honestly — it does not describe things the tool does not do.

## 1. Data controller

The data controller is the **individual who owns and operates the tool** — a single eBay seller. There is no company, no organisation, no staff and no third-party operator.

Because there is no company, controller contact details are not a postal address or phone number. To contact the controller, raise an issue on this repository.

## 2. What is collected and why

The tool handles only the following:

**Photographs of items for sale.** Sent by the operator from their own device to a private channel that only they can access. These are photos of second-hand goods being listed.

**Item details.** Titles, descriptions, condition notes and prices — generated from those photos or typed by the operator.

**The operator's own eBay account data.** Accessed with the operator's explicit consent through eBay's standard OAuth flow, limited to the `sell.inventory` scope. That permits creating and editing **the operator's own listings**. It does not permit access to payment details, account settings, or the data of any other eBay user.

**Publicly listed retail prices.** A product name (for example "RTX 3060") is looked up publicly to estimate what an item is worth. A product name is not personal data.

## 3. What is not collected

- No data belonging to buyers, customers or any other eBay user
- No payment or financial details
- No marketing lists, tracking, analytics or advertising identifiers
- No data about visitors, because there are none — the interface is on a private network behind single sign-on

There is **no cookie or tracking section**, because the tool does not set cookies and has no public website.

## 4. Lawful basis

The tool processes personal data only about the operator itself. The operator is the person the data is about, the person controlling the tool, and the only person with access — so they exercise their own data-protection rights directly over their own information on their own hardware.

Where access to a third-party system is involved, it is granted through the operator's own consent: access to the eBay account is authorised by the operator through eBay's OAuth consent screen.

This description sets out the facts of how the tool works. It is not legal advice.

## 5. Where data is stored

On hardware owned and operated by the seller, on a private network. Photographs and item records are held in a local database. **Nothing is stored with a cloud provider**, and the web interface is not reachable from the public internet.

## 6. How data is shared

Data is not sold, rented, shared or transferred to anyone for any purpose. The tool communicates with a small number of external services, sending each only what it needs to do its job:

| Service | What is sent | Why |
|---|---|---|
| **eBay** | Listing content, via the official API, with OAuth consent | To create draft listings on the operator's own account |
| **Discord** | Photographs and messages, in a private channel | Transport for sending items to the tool |
| **Price comparison sites** | A product name (e.g. "RTX 3060") | To look up publicly listed retail prices |

## 7. eBay tokens

The OAuth refresh token issued by eBay is stored locally, is never displayed in the interface, and is never transmitted anywhere except back to eBay.

Consent can be withdrawn at any time from eBay account settings, under **Site Preferences → Third-Party Authorizations**. Doing so immediately invalidates the token regardless of what this tool holds.

## 8. Retention

Photographs and item records are kept while a listing is being prepared, and for as long as the operator finds them useful as a record of what they sold. They can be deleted at any time by the operator, who is the only person with access. The tool does not operate any automatic deletion schedule.

## 9. Data subject rights

The UK GDPR gives individuals rights over their personal data — including access, rectification, erasure, restriction and portability.

**Not applicable here, and why:** the tool holds personal data only about its operator. There is no other person whose data this tool holds, so there is no third party with rights to exercise over it. The operator exercises those rights directly — they can view, correct or delete the data at any time because it is their own information on their own machine. Should that ever change, this policy will be updated before it does.

## 10. How to complain

The Information Commissioner's Office (ICO) is the UK's independent authority for data protection. If you consider that your personal data has been handled in a way that breaches UK data protection law, you have the right to complain to the ICO.

Because the tool holds no data about you, there is unlikely to be a basis for such a complaint in practice — but the right exists regardless, and the ICO's details are:

- Website: ico.org.uk
- Telephone: 0303 123 1113
- Address: Information Commissioner's Office, Wycliffe House, Water Lane, Wilmslow, Cheshire SK9 5AF

## 11. Contact

Raise an issue on this repository.