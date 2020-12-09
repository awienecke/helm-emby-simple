# helm-emby-simple

I wanted a simple chart for deploying emby, not one that had an abundance of options that made no sense for deploying it to a single node, and just so I caould run other things on the server without messing with the media server.
Mostly, I ran this so I could test jellyfin in tandem, and mission accomplished.

## Usage

Modify the values.yaml to match your servers environment, ensure the paths defined actually exist on the host and have sufficient space, ensure kubernetes is installed and you can access it, and it's the correct environment, and then simply run:

    helm install -f values.yaml emby ./

Adjust the values.yaml and ./ to the path to the helm chart if not run from inside.

