# SR Linux Asymmetric routing scenario

Simple baseline setup to play with an asymmetric IRB setup, 4 leafs and only 2 of them used by default to ensure there are enough free nodes to add more clients

---

# Client baseline setup

![pic1](https://github.com/missoso/srl-asymmetric-routing-irb/blob/main/img_and_drawio/srl-asymmetric-routing-irb.drawio.png)

# Overlay, underlay and mgmt 

![pic2](https://github.com/missoso/srl-asymmetric-routing-irb/blob/main/img_and_drawio/underlay_overlay_mgmt.drawio.png)

## Deploying the lab

The lab is deployed with the [containerlab](https://containerlab.dev) project, where [`asymmetric.clab.yml`](st.clab.yml) file declaratively describes the lab topology.

```bash
# change into the cloned directory
# and execute
containerlab deploy --reconfigure
```

To remove the lab:

```bash
containerlab destroy --cleanup
```
