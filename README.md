# 簡介
Use docker to build suricata +ELK

# 部署
1. 進到 suricata/dist/suricata.yaml 修改 suircata 的 yaml 檔
    修改 HOME_NET 成要防護的網段
2. 進到 suricata/dist/Dockerfile 修改 Dockerfile
    修改最後一行 $SURICATA_CAPTURE_FILTER -i `enp0s8` 成要監控的網卡
