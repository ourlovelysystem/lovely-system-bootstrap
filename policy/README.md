# Policy

`/policy` holds policy past, policy present, and policy future for Our Lovely System.

## Temporal scheme

- `index.html` is policy present: the policy currently in force.
- Date-qualified HTML files are policy past. When present policy is replaced, the former `index.html` is moved to a file named for the date of the transition.
- Sequence-qualified HTML files are policy future. `1.html` is next. When policy advances, `1.html` becomes `index.html`, and the remaining future files are decremented (`2.html` becomes `1.html`, `3.html` becomes `2.html`, and so on).

The epoch file is `1970-01-01.html`. It represents the initial state: no policy.

No collision mitigation is specified yet. If the simple date scheme fails in practice, that failure can be observed before a mitigation is designed.

## Policy levels

Policy may exist at several levels. Grand policy is broad system state that filters downward. Domain policy contextualizes grand policy for a domain. Ground policy applies closest to an actual system or event. Weighting and fail-open/fail-closed behavior may be expressed separately as the policy system develops.

## The ledger

The planned public steering ledger lives at `ledger.ourlovelysystem.org`.

The ledger is not merely an archive of complaints. It is intended to act as a steering control. People can use it to challenge the behavior of Our Lovely System and to put evidence, disagreement, and response into public view.

The policy process should use the ledger to inspect the epistemology of policy-making: what was believed, why it was believed, what evidence supported it, what challenged it, what assumptions survived, and what later experience showed to be wrong or incomplete.

Policy should therefore be inspectable not only as a sequence of conclusions but, where useful, as a sequence of reasons and revisions. The ledger provides a place for pressure against policy claims and for evidence that may justify changing them.

If used wisely, the ledger will steer Our Lovely System towards virtue. If abused, the ledger will produce useless noise.
