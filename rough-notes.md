```
641  docker run -d -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo -v $(pwd):/data:/var/lib/postgresql/data --name db postgres:9.4
  642  docker run -d -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo -v $(pwd)/data:/var/lib/postgresql/data --name db postgres:9.4
  643  docker run -p 8069:8069 -e DB_PORT_5432_TCP_PORT=26257 -d --link db:db odoo:11.0
  644  docker rm -f c152e064c2c84c621dde53398dbf9efe1a5f4880d340d90e5065e781a1888b76
  645  docker run -p 8069:8069  -d --link db:db odoo:11.0
  646  docker ps
  647  docker ps
  648  oc login https://stg.run9.io:8443 --token=sdfsdf-1BuQ
  649  oc adm policy add-scc-to-user anyuid -z default
  650  ssh root@stg.run9.io
  651  pwd
  652  ls
  653  pwd
  654  ls data/
  655  oc new-app https://github.com/netroby/alpine-rsync --strategy=docekr
  656  oc new-app https://github.com/netroby/alpine-rsync --strategy=docker
  657  oc new-app https://github.com/netroby/alpine-rsync --strategy=docker -h
  658  oc run -h
  659  oc run debianmaster/go-welcome --command=true
  660  oc get all
  661  oc delete all -l app=alpine-rsync
  662  oc new-build https://github.com/netroby/alpine-rsync --strategy=docker -h
  663  oc new-build https://github.com/netroby/alpine-rsync --strategy=docker
  664  oc run alpine-rsync echo test
  665  oc run alpine-rsync -- echo test
  666  oc run alpine-rsync --image=alpine-rsync -- echo test
  667  oc get po
  668  oc delete po alpine-rsync-1-zq84b
  669  oc run alpine-rsync --image=172.30.1.1:5000/web/alpine-rsync --rm -- echo test
  670  oc run alpine-rsync --image=172.30.1.1:5000/web/alpine-rsync  -- echo test
  671  oc delete dc alpine-rsync
  672  oc run alpine-rsync --image=172.30.1.1:5000/web/alpine-rsync  -- echo test
  673  oc delete all -l app=alpine-rsync
  674  oc get all --show-labels
  675  oc delete all -l run: alpine-rsync
  676  oc delete all -l run=alpine-rsync
  677  oc run alpine-rsync --image=172.30.1.1:5000/web/alpine-rsync  -- sleep 10000
  678  pwd
  679  ls
  680  oc get po
  681  oc rsync data alpine-rsync-2-5hxh7:/data
  682  oc rsync data/* alpine-rsync-2-5hxh7:/data
  683  oc rsync data/ alpine-rsync-2-5hxh7:/data
  684  ssh root@stg.run9.io
  685  oc get po
  686  oc debug db-3-hgnkd
  687  oc debug db-3-hgnkd
  688  ssh root@stg.run9.io
  689  ssh root@stg.run9.io
  690  ls
  691  ls data/
  692  oc delete all -l app=db
  693  oc get all
  694  oc get all --show-labels
  695  oc delete all -l app=postgresql-persistent
  696  oc new-app --name=db -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo docker.io/postgres:9.4
  697  ls data
  698  ls
  699  ls data/PG_VERSION
  700  cat data/PG_VERSION
  701  pwd
  702  docker ps
  703  docker exec -it 38f084dea2aa sh
  704  ls
  705  docker cp 38f084dea2aa:/var/lib/odoo .
  706  docker cp 38f084dea2aa:/var/lib//mnt/extra-addons .
  707  docker cp 38f084dea2aa:/mnt/extra-addons .
  708  ls
  709  pwd
  710  ls
  711  oc get po
  712  oc cp odoo/ run9-5-dmmkz:/var/lib/odoo
  713  oc cp odoo/ run9-5-dmmkz:/tmp/odoo
  714  oc cp extra-addons/ run9-5-dmmkz:/tmp/extra-addons
  715  oc get po
  716  oc rsh run9-5-dmmkz
  717  oc get po
  718  oc rsync odoo alpine-rsync-4-7rstl:/odoo
  719  oc rsync odoo/* alpine-rsync-4-7rstl:/odoo
  720  oc rsync odoo/ alpine-rsync-4-7rstl:/odoo
  721  oc rsync extra-addons/ alpine-rsync-4-7rstl:/extra-addons
  722  oc get po
  723  oc rsh alpine-rsync-4-nfg92 chown -R 101:101 /odoo
  724  oc rsh alpine-rsync-4-nfg92 chown -R 101:101 /extra-addons
  725  oc get po
  ```
