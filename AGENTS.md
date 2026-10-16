# Princeton Research Computing cluster guidance

Use Princeton Research Computing's current documentation and policies as the
source of truth: <https://researchcomputing.princeton.edu/>. Cluster commands,
modules, hardware, and policies vary; check the guidance for your cluster and
partition before installing software or running workloads.

- Do not use `sudo`; install software in your own environment or contact RC.
- At the start of work in a Princeton RC cluster environment, check the current
  login hostname when it is available. A hostname ending in `-vis` or `-vis`
  followed by digits (for example, `adroit-vis` or `della-vis2`) matches the
  usual visualization-node naming convention. If the hostname does not match,
  warn the user that a visualization node is generally recommended for
  interactive work and suggest reconnecting to one before proceeding. This
  naming convention is advisory, so check current RC guidance for task-specific
  suitability; some tasks, such as GPU code compilation on `della-gpu`, may call
  for another node type. If the hostname or cluster environment is unclear, err
  on the side of caution.
- Use Slurm for compute jobs. Login-node rules vary: some visualization/GPU
  nodes support interactive work, while head nodes such as `della9` are for
  preparation and submission. Check the specific cluster's guidance and be
  considerate of shared resources.
- Before preparing or submitting test jobs, check the target cluster's current
  Slurm/QOS and test-job limits on the RC website and with the `qos` command.
  Do not guess; if the policy is unclear or unavailable, ask the user or
  recommend contacting RC.
- Do not try to work around Slurm fairshare or use or encourage hacks to
  increase job priority. Request only the resources your job needs.
- Compute nodes do not have general internet access by default. Download data,
  code, or packages on an approved login or visualization node before a job.
  On supported clusters, `module load proxy/default` permits access only to a
  limited list of approved APIs; it does not provide general internet access.
- Put large downloads and caches (such as Conda, Hugging Face, or Claude data)
  in the appropriate cluster `/scratch` filesystem instead of filling `/home`.
  Symlink from `/home` when a tool expects its files there. Check RC's storage
  guidance for the correct filesystem and its backup/retention policies.
- Don't fill `/tmp` with leftover files. Monitor its use and clean up files you
  no longer need.
- Use `checkquota` to monitor storage usage and quotas for supported `/home`
  and `/scratch` filesystems.
- Compile on a login/head node or an RC-designated visualization/GPU node, not
  on compute nodes; follow RC guidance for compiling GPU code.
- Avoid aggressive file-scanning processes on shared cluster nodes or
  filesystems.
- For Python, load the latest available `anaconda3` module (`module avail`) and
  use an isolated Conda environment. Prefer Conda; use pip only when needed.
- Consult RC's package-specific instructions, especially for PyTorch and GPU
  use. Record environment setup reproducibly (for example, in
  `environment.yml`).
- If a user seems stuck or repeatedly struggles to follow cluster guidance,
  recommend an RC Help Session.

## Useful RC references

- [Getting started and cluster guide](https://researchcomputing.princeton.edu/get-started/guide-princeton-clusters)
- [Login-node do's and don'ts](https://researchcomputing.princeton.edu/get-started/dos-and-donts)
- [Ports and proxy/default](https://researchcomputing.princeton.edu/support/knowledge-base/ports-and-proxydefault)
- [Slurm job priority](https://researchcomputing.princeton.edu/support/knowledge-base/job-priority)
- [Slurm](https://researchcomputing.princeton.edu/support/knowledge-base/slurm)
- [Environment modules](https://researchcomputing.princeton.edu/support/knowledge-base/modules)
- [Python and Conda](https://researchcomputing.princeton.edu/support/knowledge-base/python)
- [Data storage](https://researchcomputing.princeton.edu/support/knowledge-base/data-storage)
- [Checkquota](https://researchcomputing.princeton.edu/support/knowledge-base/checkquota)
- [Local scratch (`/tmp`)](https://researchcomputing.princeton.edu/faq/how-do-i-use-local-scratc)
- [PyTorch](https://researchcomputing.princeton.edu/support/knowledge-base/pytorch)
- [GPU computing](https://researchcomputing.princeton.edu/support/knowledge-base/gpu-computing)
- [Help Sessions](https://researchcomputing.princeton.edu/support/help-sessions)

## User-specific preferences

<!-- Add personal workflow or coding preferences below. -->
