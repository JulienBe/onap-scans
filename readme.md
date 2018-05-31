## Empty folders

`for i in *; do echo "$i"; find "$i" | grep -v "/.git" | wc -l; done | grep "^1$" -B1 | grep -v "^1$\|--"`

    cla
    dcaegen2_analytics_flink
    dcaegen2_analytics_pnda
    dcaegen2_platform_registrator
    doc_tools
    integration_seccom
    multicloud_k8s
    multicloud_openstack_windriver
    optf_cmso
    sdc_dcae-d_rule-engine
    sdnc_apps
    sdnc_architecture
    sdnc_parent
    university
    vnfrqts_epics
    vvp_ansible-ice-bootstrap
