# Tensorboard

- open server tensorboard in local
  - ssh -L 16006:127.0.0.1:6006 username@remote_server_ip
  - in server: *tensorboard* --*logdir=xxx* --*port=6006*
  - in local browser: 127.0.0.1:16006