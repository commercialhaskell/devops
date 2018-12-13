# Set kubeconfig for new deployments (usually this will be prod).
# helm=TILLER_NAMESPACE="kube-system" KUBECONFIG="" helm
NAME=commercialhaskell-com-redirect

apply:
	$(helm) upgrade --install $(NAME) .

delete:
	$(helm) delete $(NAME)

purge:
	$(helm) del --purge $(NAME)

list:
	$(helm) list

version:
	$(helm) version

update:
	$(helm) repo update

ls:
	$(helm) ls --all $(NAME)

template:
	$(helm) template .

status:
	$(helm) status $(NAME)
