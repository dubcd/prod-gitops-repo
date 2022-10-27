# prod-gitops-repo
ssh-keygen -f gitops-secret -t ed25519

flux create secret git gitops-secret-auth \
    --url=ssh://git@github.com/anakhub/secretrepo \
    --private-key-file=./gitops-secret