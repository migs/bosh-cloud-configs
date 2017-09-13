# bosh-scripts

## Fresh bosh director first steps:

```
git clone https://github.com/migs/bosh-scripts.git
bosh ucc bosh-scripts/cloud-configs/gcp/europe-west2.yml -n
bosh upload-stemcell https://bosh.io/d/stemcells/bosh-google-kvm-ubuntu-trusty-go_agent
bosh upload-release https://storage.googleapis.com/bosh-gcp/beta/stackdriver-tools/latest.tgz --non-interactive
bosh update-runtime-config bosh-scripts/runtime-config.yml
```
