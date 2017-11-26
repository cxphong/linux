#### 1. **Sample service**

  ```bash
  # turn.service
  [Unit]
  Description=Turn server
  After=network-online.target

  [Service]
  ExecStart=/usr/local/bin/turnserver
  Restart=always
  RestartSec=10s

  [Install]
  WantedBy=multi-user.target
  ```
  
#### 2. **Add new serivce**

  ```bash
  sudo cp turn.service /lib/systemd/system
  sudo systemctl daemon-reload
  ```
  
#### 3. **Opertion**

  ```bash
  sudo systemctrl restart/start/stop/status turn
  ```

#### 4. **Log**

  ```bash
  sudo journal -u turn
  ```
