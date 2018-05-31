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

# Failed jobs

        aaf_cadi-checkmarx
        aaf_inno-checkmarx
        aai_eis-checkmarx
        aai_gap-checkmarx
        aai_graphadmin-checkmarx
        aai_graphgraph-checkmarx
        aai_spike-checkmarx
        aai_tabular-data-service-checkmarx
        ccsdk_parent-checkmarx
        ccsdk_platform_blueprints-checkmarx
        ccsdk_storage_pgaas-checkmarx
        ccsdk_utils-checkmarx
        cla-checkmarx
        dcae-checkmarx
        dcae_apod-checkmarx
        dcae_collectors-checkmarx
        dcae_demo_startup-checkmarx
        dcae_demo_startup_aaf-checkmarx
        dcae_demo_startup_controller-checkmarx
        dcae_operation-checkmarx
        dcae_utils-checkmarx
        dcae_utils_buildtools-checkmarx
        dcaegen2-checkmarx
        dcaegen2_analytics-checkmarx
        dcaegen2_analytics_flink-checkmarx
        dcaegen2_analytics_pnda-checkmarx
        dcaegen2_collectors-checkmarx
        dcaegen2_platform-checkmarx
        dcaegen2_platform_registrator-checkmarx
        doc_tools-checkmarx
        integration_seccom-checkmarx
        modeling_modelspec-checkmarx
        multicloud_azure-checkmarx
        multicloud_k8s-checkmarx
        multicloud_openstack_windriver-checkmarx
        music_mdbc-checkmarx
        music_prom-checkmarx
        ncomp-checkmarx
        ncomp_sirius-checkmarx
        onap-checkmarx
        oparent-checkmarx
        optf_cmso-checkmarx
        policy_apex-pdp-checkmarx
        policy_api-checkmarx
        policy_core-checkmarx
        policy_distribution-checkmarx
        policy_gui-checkmarx
        policy_models-checkmarx
        policy_pap-checkmarx
        policy_parent-checkmarx
        policy_pdp-checkmarx
        policy_xacml-pdp-checkmarx
        sdc_dcae-d_rule-engine-checkmarx
        sdc_onap-ui-checkmarx
        sdc_sdc-docker-base-checkmarx
        sdnc_adaptors-checkmarx
        sdnc_apps-checkmarx
        sdnc_architecture-checkmarx
        sdnc_core-checkmarx
        sdnc_parent-checkmarx
        sdnc_plugins-checkmarx
        ui-checkmarx
        university-checkmarx
        vnfrqts_epics-checkmarx
        vnfrqts_guidelines-checkmarx
        vvp_ansible-ice-bootstrap-checkmarx
        vvp_documentation-checkmarx
