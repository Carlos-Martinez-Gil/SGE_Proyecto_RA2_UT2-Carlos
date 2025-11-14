# 08 — Servicio systemd (`odoo.service`)

1. Crea el servicio en `/etc/systemd/system/odoo.service`:
   ```ini
   [Unit]
   Description=Odoo Service
   After=network.target postgresql.service

   [Service]
   Type=simple
   User=odoo
   Group=odoo
   ExecStart=/opt/odoo/venv/bin/python /opt/odoo/odoo-src/odoo-bin -c /etc/odoo/odoo.conf
   Restart=on-failure

   [Install]
   WantedBy=multi-user.target
   ```
2. Recarga y arranca:
   ```bash
   sudo systemctl daemon-reload
   sudo systemctl enable --now odoo
   sudo systemctl status odoo
   ```

![systemd](../assets/img/08-servicio_systemd/paso01_status-odoo.png "Estado de systemd")

> Resultado esperado: servicio `odoo` activo y habilitado.

- Entro en el fichero con "sudo nano /etc/systemd/system/odoo.service"
- Edito el fichero con estos contenidos
   ![](../assets/img/08-servicio_systemd/fichero.png)

- Recargo el systemctl con estos comandos "sudo systemctl daemon-reload" "sudo systemctl enable --now odoo" "sudo systemctl status odoo"
   ![](../assets/img/08-servicio_systemd/recargar.png)
