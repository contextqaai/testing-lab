# Infor enterprise lab

**Route:** Product-specific customer/partner test tenant

## What is established

Choose the actual product, such as CloudSuite Industrial, M3 or LN, and obtain an authorized nonproduction tenant. A generally available self-service full-ERP sandbox was not established by this assessment.

Infor OS Portal is a browser entry point for integrated applications; app access depends on identity, roles and product configuration. Public design-system components alone do not reproduce an ERP workflow.

## Current boundary

No Infor tenant or runtime is verified. No product-wide compatibility claim is made.

## Proposed first exercise

Proposed after product selection: find a synthetic item/order, perform one allowed status transition and verify the changed state. This is a blueprint, not an implemented tenant workflow or execution receipt.

## Access handoff

- Exact Infor product and version
- Authorized test tenant and product permissions
- Dedicated test user and synthetic records
- Allowed UI/API workflow and reset procedure

## Sources checked October 25, 2026

- https://developer.infor.com/tutorials/portal-and-workspaces
- https://developer.infor.com/tutorials/security-and-user-management/67d82a566ec13166516df081

No signup, agreement acceptance, paid provisioning or change to an existing enterprise tenant was performed.
