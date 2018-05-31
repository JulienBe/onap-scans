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

## Python friendly repos

`find ./ -name "*.py" | cut -d'/' -f 2 | uniq -c | sort -n -r`

    264 multicloud_openstack
    250 vvp_engagementmgr
    176 vfc_nfvo_lcm
    166 multicloud_openstack_vmware
    141 optf_has
    105 vvp_test-engine
     83 vnfsdk_dovetail-integration
     80 modeling_toscaparsers
     76 vnfsdk_ice
     72 vfc_gvnfm_vnflcm
     70 vvp_validation-scripts
     61 optf_osdf
     53 so
     52 vfc_nfvo_catalog
     50 multicloud_framework
     50 dcaegen2_platform_plugins
     50 dcaegen2_platform_cli
     49 sdc
     43 sdc_dcae-d_tosca-lab
     32 vfc_gvnfm_vnfres
     32 vfc_gvnfm_vnfmgr
     29 dcaegen2_utils
     27 vvp_cms
     27 ccsdk_platform_plugins
     26 dcaegen2_platform_policy-handler
     25 integration
     23 vfc_nfvo_driver_vnfm_svnfm
     23 oom
     21 vfc_nfvo_driver_vnfm_gvnfm
     20 dcaegen2_services_heartbeat
     20 dcaegen2_collectors_snmptrap
     16 vnfsdk_pkgtools
     16 testsuite_python-testing-utils
     12 vvp_image-scanner
     10 dcaegen2_platform_configbinding
      9 logging-analytics
      7 testsuite_heatbridge
      7 appc
      6 sdnc_oam
      6 demo
      5 testsuite_properties
      4 vnfsdk_ves-agent
      4 vnfsdk_compliance
      4 ccsdk_sli_adaptors
      3 sdc_dcae-d_ci
      3 dcae_pgaas
      2 sdnc_northbound
      2 sdc_jtosca
      2 integration_devtool
      2 doc
      2 dcaegen2_deployments
      2 clamp
      1 vvp_documentation
      1 vvp_devkit
      1 vnfrqts_usecases
      1 vnfrqts_testcases
      1 vnfrqts_requirements
      1 testsuite
      1 so_docker-config
      1 policy_engine
      1 oom_registrator
      1 music_prom
      1 mso_docker-config
      1 dcae_controller
      1 dcae_apod_cdap
      1 ccsdk_distribution
      1 appc_deployment
