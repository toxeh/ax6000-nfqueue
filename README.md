# ax6000-nfqueue

Модуль ядра и библиотеки для поддержки `nfqueue` в iptables.
Установка через `opkg` с включенным overlay.

  ```
  opkg update
  opkg install ./iptables-mod-nfqueue_1.6.2-3_aarch64_cortex-a53.ipk \
   ./kmod-ipt-core_4.4.60-1_aarch64_cortex-a53.ipk \
   ./kmod-ipt-nfqueue_4.4.60-1_aarch64_cortex-a53.ipk \
   ./kmod-nf-ipt_4.4.60-1_aarch64_cortex-a53.ipk \
   ./kmod-nf-reject_4.4.60-1_aarch64_cortex-a53.ipk \
   ./kmod-nfnetlink-queue_4.4.60-1_aarch64_cortex-a53.ipk \
   ./kmod-nfnetlink_4.4.60-1_aarch64_cortex-a53.ipk
  ```

Загрузка модуля ядра
  ```
  insmod xt_NFQUEUE