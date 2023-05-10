# gke-rightsize

gcloud projects add-iam-policy-binding PROJECT_ID --member="user:EMAIL_ADDRESS" --role=ROLE

gcloud projects add-iam-policy-binding agmsb-gke-lab --member="user:agmsb@cloudadvocacyorg.joonix.net" --role=roles/serviceusage.serviceUsageAdmin

gcloud projects add-iam-policy-binding agmsb-gke-lab --member="user:agmsb@cloudadvocacyorg.joonix.net" --role=roles/container.clusterAdmin

gcloud projects add-iam-policy-binding agmsb-gke-lab --member="user:agmsb@cloudadvocacyorg.joonix.net" --role=roles/iam.serviceAccountAdmin

gcloud projects add-iam-policy-binding agmsb-gke-lab --member="user:agmsb@cloudadvocacyorg.joonix.net" --role=roles/iam.securityAdmin

gcloud projects add-iam-policy-binding agmsb-gke-lab --member="user:agmsb@cloudadvocacyorg.joonix.net" --role=roles/container.admin

export PROJECT_ID=agmsb-gke-lab
export REGION=us-central1
export ZONE=us-central1-f

gcloud config set project agmsb-gke-lab

git clone https://github.com/GoogleCloudPlatform/kubernetes-engine-samples

cd kubernetes-engine-samples/gke-vpa-recommendations

./scripts/setup.sh