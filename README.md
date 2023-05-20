# Ingress domain rewriter

If you want to run the same infra on different domains, this might be a solution for you!

# Intended Usage
## Sharing gitops structures
Main focus is on being able to share and package larger gitops:ed infra definitions. These often include an Ingress definition in real life and with this operator you can easily adapt the ingress definitions to fit different base domains.

## Blue green deployments
Imagine having blue green deployments and you want to gitops the same folders. But you might want to run some system tests before you switch over from one system to another. This will allow you to change the base domain on the fly for the non-active cluster to run these system tests. Then you can switch back before you switch cluster.

## More?
If you find some cool use-case for it, feel free to PR.
