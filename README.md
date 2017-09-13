# bosh-scripts

## Fresh bosh director first steps:

```
git clone https://github.com/migs/bosh-scripts.git
yes | bosh ucc bosh-scripts/cloud-config/gcp/europe-west2.yml
bosh upload-stemcell https://bosh.io/d/stemcells/bosh-google-kvm-ubuntu-trusty-go_agent
bosh upload-release https://storage.googleapis.com/bosh-gcp/beta/stackdriver-tools/latest.tgz --non-interactive
```
