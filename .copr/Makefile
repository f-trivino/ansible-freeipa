srpm:
	# Setup development environment
	echo "Installing base development environment"
	dnf install -y dnf-plugins-core wget git-all
	echo "Call SRPM build Script"
	./utils/build-srpm-twoerner.sh
	if [[ "${outdir}" != "" ]]; then \
		mv /builddir/build/SRPMS/* ${outdir}; \
	fi
