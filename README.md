### Helm Chart for Logistics Wizard

1. Create Standard/Paid cluster on IKS and set up kubectl and run `helm init`
2. Open `logistics-wizard/values.yaml` and update `hosts` field with your Ingress subdomain.
```
  hosts:
    - mycluster-472085.us-south.containers.appdomain.cloud
```
3. `helm install --name mylw ./logistics-wizard/`