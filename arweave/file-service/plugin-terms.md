[Homepage](../../) / [Partner: Arweave](../) / [Mask Network Plugin "File Service"](./) / Terms of Use

# Mask Network Plugin "Web3 File Service"

# Terms of Use

Last Updated on Dec 09, 2022

## Introduction

This is the terms of use for Mask Network Plugin "Web3 File Service" and the online service behind it. This Terms of Use is subject to the Mask Network Service Agreement.

This service is powered by Mask Network's partner file storage protocols such as IPFS and Arweave.

## Definitions

- This service: Web3 File Service hereby being described.

- We: The maintainer of this service, i.e.Dimension.io.

- You: The end user hereby using this service.

- File Storage Protocols: Mask Networks's partner file storage protocols include IPFS and Arweave. At your choice, you could select one to complete your use of Web3 File Service.

## Coverage

This document includes the terms of using the Mask Network Plugin "Web 3 File Service" (com.maskbook.fileservice). Mask Network itself and other plugins are not covered here.

## Copyright

- You should be the appropriate copyright owner or an authorized person/organization when uploading a file.

- When uploading, you implicitly permit mask.io and other partnered File Storage Protocols and any node in the file service network to service verbatim copies of file over Internet, to the extent necessary for allowing you to share the file.

## Persistence

- Once you have uploaded a file, it may be impossible to delete it, because the storage is built over blockchain technologies.

- If you request to remove a file, such removal request may or may not be fulfilled.

## Liability

- You are solely responsible for not violating the law when using this service. This service does not assume any liability for any event, e.g. loss of data & damage of business interest.

## Law Enforcement

- This service is a combination of multiple independent sub-services. The providers of these sub-services (including and without limitation to Mask Network and File Storage Protocols) may comply with court orders and search warrants from law enforcement authorities.

## Technical Summary

### Uploading

This Plugin encrypts the selected file with an AES-256-GCM Key (FileKey) to get Encrypted File (EF) and publishes EF on the file storage protocols. File storage protocols provide a file storage service and an HTTPS interface to retrieve stored files. Also, this Plugin generates a Landing Page (LP) which contains the HMAC-SHA256 hash (HH) of the FileKey (for verification), and publishes it via File Storage Protocols. The Plugin writes FileKey and the URL of the LP into the Post, so that everyone who can decrypt the post can visit the Landing Page.

### Downloading

When clicking "Download File" in the Snippet under the Post, Mask Network will open the Landing Page. The Landing Page requests all active tabs in the browser to present the FileKey. Mask Network will receive this request and will provide the FileKey.

The Landing Page gets the FileKey and tries verifying the given FileKey with HH. If it is correct, the Landing Page will download the EF from File Storage Protocols and will decrypt it. The visitor can then preview it and save it to the local machine.

## Miscellaneous Disclaimers

- Due to technical limitations, the upload progress cannot be very accurate.

- The definition of file size units (MB, KB, etc) can be platform-specific. Some systems use [1000-based definitions](https://en.wikipedia.org/wiki/Metric_prefix), while others use [1024-based definitions](https://en.wikipedia.org/wiki/Binary_prefix). You may see different sizes for the same file.

- This service does not manage any data beyond the range specified in this document. Mask Network the software might manage other necessary data, and is beyond the control of this Plugin and/or this Service.

## Changes to this Statement / Contact Us

We may update these terms without explicit notifications. You should frequently check if there is any update, especially after updating Mask Network versions.

If you have any questions about this policy, please contact [support@mask.io](mailto:support@mask.io).
