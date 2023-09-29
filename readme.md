<h1>How to run</h1>
<h2>1- Custom</h2>
<p>
- Edit all pvs yml an change value of kubernetes host.<br/>
Sample:
          - key: kubernetes.io/hostname<br/>
            operator: In<br/>
            values:<br/>
              - shermine237-latitudee6410<br/>
</p>
<h2>2- Set volumes</h2>
<p>
- Go to "/" folder : <code>cd /</code><br/>
- Clone k8s volume: <code>sudo git clone https://github.com/Shermine237/k8s_storages_volumes.git</code><br/>
- Change user own: <code>sudo chown user:user k8s_storages_volumes</code><br/>
- Rename: <code>sudo mv k8s_storages_volumes k8s-volumes</code><br/>
- Create these folder if not exit:<br/>
<code>mkdir /k8s-volumes/odoo/addons</code><br/>
<code>mkdir /k8s-volumes/odoo/web-data</code><br/>
</p>
<h2>3- Apply files in order</h2>
<p>
See order-to-apply.txt<br/>
</p>
