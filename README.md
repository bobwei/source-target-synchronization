# Source Target Synchronization

- [Flow](#flow)
- [How to sync between source and target ?](#how-to-sync-between-source-and-target-?)
- [Example](#example)


## Flow
- diff
- push
- merge


## How to sync between source and target ?

- Maintain a currentState which is synchronized with local source and contains a list of ids of the source.
- Assume there is a cron job executed for every time T.
- When job executed, do the followings:
  - Compare local source with currentState to calculate diff
  - If diff exists, push diff
- When receive diff from other sources, merge diff into local source.
  - Merge Strategy:
    - create => insert
    - remove => delete
    - update => compare updatedTime, merge with the largest updatedTime


## Example

We use snapshots at each time t to illustrate this algorithm, please checkout examples for further detail.
- example1
  - t0
    - [source](./examples/example0/t0/source.md)
    - [target](./examples/example0/t0/target.md)
  - t1
    - [source](./examples/example0/t1/source.md)
    - [target](./examples/example0/t1/target.md)
  - t2
    - [source](./examples/example0/t2/source.md)
    - [target](./examples/example0/t2/target.md)
