NAME=cert-manager
NAMESPACE=cozy-$(NAME)

include ../../../hack/package-system.mk

update:
	rm -rf charts
	helm repo add jetstack https://charts.jetstack.io
	helm repo update jetstack
	helm pull jetstack/cert-manager --untar --untardir charts
