# [Kubernetes](https://kubernetes.io/)

## Notes

- Kubernetes runs pods that contain 1 to n docker containers. So if you have your apps in the form of docker images you are ready to go.
- [The OpenShift guys like to make the analogy that Kubernetes is like Linux and that there are different distributions of it, OpenShift being one (like Red Hat).](https://www.reddit.com/r/devops/comments/94n994/for_those_of_you_who_use_kubernetes_how_the_hell/)
- [Interacting with kubernetes feels very different and in a lot of ways it's almost an operating system for a super computer. You sort of forget how many computers and vms or whatever are out there and kubernetes handles a lot of the implementation details for you. Installing a lot of apps to the cloud is as simple as typing 'helm install jenkins' and waiting 5 minutes.](https://www.reddit.com/r/investing/comments/92becj/is_amazon_undervalued_with_the_huge_aws_earnings/)
  - It's just a radically new way of dealing with 'the cloud'. And the thing that makes it especially threatening to aws is that it doesn't matter where it runs. Developing an app for kubernetes on aws or google cloud or azure or anything else is almost an identical experience. People are going to become very price sensitive because that's the only thing that distinguishes one kubernetes host from another (aside from the ease of installing a kubernetes cluster -- something which aws is fairly far behind on)
- In general, the right question to ask yourself when designing Pods is, “Will these containers work correctly if they land on different machines?” If the answer is “no,” a Pod is the correct grouping for the containers. If the answer is “yes,” multiple Pods is probably the correct solution.
- Ingress controller watches for `Ingress` resources in your cluster.
- [Kubernetes (or whatever other container scheduler) might feel like overkill, but if all they do is force you to adopt a container-centric / 12-factor way of building your applications it was worth trying them. And once you've adopted that workflow it's a no-brainer to go from a single node to a cluster which will dynamically allocate the workloads it runs.](https://news.ycombinator.com/item?id=18495697)
  - Running a small container cluster at work has even changed how I setup single-host projects in my spare time: I will build everything into a container, bind-mount whatever it might need, create a simple systemd unit that just runs / rms the docker container on start and stop. Bliss.

## Links

- [What happens when I type kubectl run](https://github.com/jamiehannaford/what-happens-when-k8s)
- [Helm](https://helm.sh/) - Kubernetes package manager.
- [Kubernetes Security - Best Practice Guide](https://github.com/freach/kubernetes-security-best-practice)
- [kaniko](https://github.com/GoogleContainerTools/kaniko) - Build Container Images In Kubernetes.
- [Draft](https://github.com/azure/draft) - Streamlined Kubernetes Development.
- [Nix Kubernetes](https://github.com/xtruder/nix-kubernetes) - Kubernetes deployment manager written in Nix.
- [Knative Serving](https://github.com/knative/serving#readme) - Kubernetes-based, scale-to-zero, request-driven compute.
- [Rancher](https://rancher.com/kubernetes/)
- [OpenShift](https://www.openshift.com/)
- [Portainer](https://portainer.io) - Lighter than Rancher (for Docker).
- [Kubernetes 101 (2018)](https://www.stavros.io/posts/kubernetes-101/)
- [node-problem-detector](https://github.com/kubernetes/node-problem-detector) - Aims to make various node problems visible to the upstream layers in cluster management stack.
- [kubectx](https://github.com/ahmetb/kubectx) - Fast way to switch between clusters and namespaces in kubectl.
- [Kubernetes for Sysadmins – Kelsey Hightower (2016)](https://www.youtube.com/watch?v=HlAXp0-M6SY)
- [Kubernetes API conventions](https://github.com/kubernetes/community/blob/master/contributors/devel/api-conventions.md#readme)
- [Kubeval](https://github.com/garethr/kubeval#readme) - Validate your Kubernetes configuration files, supports multiple Kubernetes versions.
- [Let's encrypt with GKE instructions](https://github.com/ahmetb/gke-letsencrypt#readme)
- [Kubernetes for personal projects? No thanks! (2018)](http://carlosrdrz.es/kubernetes-for-small-projects/)
- [Kubespy](https://github.com/pulumi/kubespy#readme) - Tools for observing Kubernetes resources in real time, powered by Pulumi.
- [Terraform Kubernetes provider](https://github.com/terraform-providers/terraform-provider-kubernetes)
- [KubeContext](https://github.com/turkenh/KubeContext) - Menu Bar App for Managing Kubernetes Contexts on Mac.
- [Kubeapps](https://github.com/kubeapps/kubeapps) - Web-based UI for deploying and managing applications in Kubernetes clusters.
- [kubefwd](https://github.com/txn2/kubefwd) - Bulk port forwarding Kubernetes services for local development.
- [You might not need Kubernetes (2018)](https://blog.jessfraz.com/post/you-might-not-need-k8s/) - [HN](https://news.ycombinator.com/item?id=18495697)
- [Kubespray](https://github.com/kubernetes-incubator/kubespray) - Deploy a Production Ready Kubernetes Cluster.
- [Argo](https://github.com/argoproj/argo) - Container-native workflows for Kubernetes.
- [Kazan](https://github.com/obmarg/kazan) - Kubernetes API client for Elixir.
- [Tilt](https://github.com/windmilleng/tilt) - Local Kubernetes development with no stress.
- [Maestro](https://github.com/maestrosdk/maestro) - Provides a declarative approach to building production-grade Kubernetes Operators covering the entire application lifecycle.
- [kail](https://github.com/boz/kail) - Kubernetes log viewer.