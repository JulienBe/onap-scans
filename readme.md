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

`find ./ -name "*.py" | cut -d'/' -f 2 | uniq -c | sort -k 2`
      7 appc
      1 appc_deployment
      1 ccsdk_distribution
     27 ccsdk_platform_plugins
      4 ccsdk_sli_adaptors
      2 clamp
      1 dcae_apod_cdap
      1 dcae_controller
     20 dcaegen2_collectors_snmptrap
      2 dcaegen2_deployments
     50 dcaegen2_platform_cli
     10 dcaegen2_platform_configbinding
     50 dcaegen2_platform_plugins
     26 dcaegen2_platform_policy-handler
     20 dcaegen2_services_heartbeat
     29 dcaegen2_utils
      3 dcae_pgaas
      6 demo
      2 doc
     25 integration
      2 integration_devtool
      9 logging-analytics
     80 modeling_toscaparsers
      1 mso_docker-config
     50 multicloud_framework
    264 multicloud_openstack
    166 multicloud_openstack_vmware
      1 music_prom
     23 oom
      1 oom_registrator
    141 optf_has
     61 optf_osdf
      1 policy_engine
     49 sdc
      3 sdc_dcae-d_ci
     43 sdc_dcae-d_tosca-lab
      2 sdc_jtosca
      2 sdnc_northbound
      6 sdnc_oam
     53 so
      1 so_docker-config
      1 testsuite
      7 testsuite_heatbridge
      5 testsuite_properties
     16 testsuite_python-testing-utils
     72 vfc_gvnfm_vnflcm
     32 vfc_gvnfm_vnfmgr
     32 vfc_gvnfm_vnfres
     52 vfc_nfvo_catalog
     21 vfc_nfvo_driver_vnfm_gvnfm
     23 vfc_nfvo_driver_vnfm_svnfm
    176 vfc_nfvo_lcm
      1 vnfrqts_requirements
      1 vnfrqts_testcases
      1 vnfrqts_usecases
      4 vnfsdk_compliance
     83 vnfsdk_dovetail-integration
     76 vnfsdk_ice
     16 vnfsdk_pkgtools
      4 vnfsdk_ves-agent
     27 vvp_cms
      1 vvp_devkit
      1 vvp_documentation
    250 vvp_engagementmgr
     12 vvp_image-scanner
    105 vvp_test-engine
     70 vvp_validation-scripts

# Failed jobs

        ccsdk_storage_pgaas-checkmarx               . ./docs ./docs/index.rst ./pom.xml ./version.properties ./bin ./bin/repackage ./README.md ./INFO.yaml ./makefile ./LICENSE.txt
        multicloud_openstack_windriver-checkmarx    EMPTY
        dcaegen2_platform_registrator-checkmarx     EMPTY
        vvp_ansible-ice-bootstrap-checkmarx         EMPTY
        dcaegen2_analytics_flink-checkmarx          EMPTY
        dcaegen2_analytics_pnda-checkmarx           EMPTY
        sdc_dcae-d_rule-engine-checkmarx            EMPTY
        integration_seccom-checkmarx                EMPTY
        sdnc_architecture-checkmarx                 EMPTY
        multicloud_k8s-checkmarx                    EMPTY
        vnfrqts_epics-checkmarx                     EMPTY
        sdnc_parent-checkmarx                       EMPTY
        university-checkmarx                        EMPTY
        doc_tools-checkmarx                         EMPTY
        optf_cmso-checkmarx                         EMPTY
        sdnc_apps-checkmarx                         EMPTY
        cla-checkmarx                               EMPTY
        sdc_onap-ui-checkmarx                       find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> babelrc ts json js md sample pack idx html npmignore xml editorconfig scss properties eslintrc yaml css txt svg TXT yml snap png
        sdc_sdc-docker-base-checkmarx               find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> /base_sdc-python/Dockerfile /base_sdc-vnc/Dockerfile rst sample /base_sdc-cassandra/Dockerfile /base_sdc-cqlsh/Dockerfile xml /base_sdc-sanity/Dockerfile properties /base_sdc-kibana/Dockerfile /base_sdc-elasticsearch/Dockerfile yaml txt /base_sdc-jetty/Dockerfile sh
        vnfrqts_guidelines-checkmarx                find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> jpg docx rst png sample txt ini
        dcaegen2-checkmarx                          find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> png graffle md /platformdoc/Dockerfile yml gif rst yaml swp swo sample idx pack sh xml properties txt
        modeling_modelspec-checkmarx                find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> rst JPG sample idx pack yaml txt
        vvp_documentation-checkmarx                 find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> rst py sample txt yaml ini
        policy_apex-pdp-checkmarx                   find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> sample pack idx xml java g4 txt xsd json junk funkylogic properties md yaml <=-
        music_prom-checkmarx                        find . -type f | awk -F. '!a[$NF]++{print $NF}' | grep -v git | xargs echo> sample xml /Dockerfile md yaml sh java properties failure cluster py json failover standby monitor txt <=-
        sdnc_adaptors-checkmarx                     find . -type f | grep -v "\.git" | xargs echo | sed -e "s#\./##g"> aai-service/README.md pom.xml sql-resource/README.md resource-assignment/.sonar/pmd.xml resource-assignment/.sonar/checkstyle.xml resource-assignment/README.md version.properties README.md mdsal-resource/README.md LICENSE.txt
        sdnc_plugins-checkmarx                      find . -type f | grep -v "\.git" | xargs echo | sed -e "s#\./##g"> properties-node/README.md pom.xml restapi-call-node/README.md version.properties README.md LICENSE.txt
        sdnc_core-checkmarx                         find . -type f | grep -v "\.git" | xargs echo | sed -e "s#\./##g"> sliapi/README.md pom.xml filters/README.md sliPluginUtils/README.md .scanignore version.properties README.md rootpom/pom.xml rootpom/README.md sli/README.md dblib/README.md src/site/apt/nodes.apt src/site/site.xml LICENSE.txt
        policy_api-checkmarx                        INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        policy_gui-checkmarx                        INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        policy_pap-checkmarx                        INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        policy_core-checkmarx                       INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        policy_models-checkmarx                     INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        policy_xacml-pdp-checkmarx                  INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        policy_distribution-checkmarx               INFO.yaml  LICENSE.txt  pom.xml  README.md  version.properties
        aai_eis-checkmarx                           INFO.yaml only
        aai_gap-checkmarx                           INFO.yaml only
        aai_spike-checkmarx                         INFO.yaml only
        music_mdbc-checkmarx                        INFO.yaml only
        aai_graphadmin-checkmarx                    INFO.yaml only
        aai_graphgraph-checkmarx                    INFO.yaml only
        multicloud_azure-checkmarx                  INFO.yaml only
        aai_tabular-data-service-checkmarx          INFO.yaml only
        policy_pdp-checkmarx                        integration/pom.xml pom.xml version.properties README.md INFO.yaml LICENSE.txt
        policy_parent-checkmarx                     ./integration/pom.xml ./pom.xml ./version.properties ./README.md ./INFO.yaml ./LICENSE.txt
        dcaegen2_platform-checkmarx                 LICENSE.txt  mvn-phase-lib.sh*  mvn-phase-script.sh*  pom.xml  version.properties
        dcaegen2_analytics-checkmarx                LICENSE.txt  mvn-phase-lib.sh*  mvn-phase-script.sh*  pom.xml  version.properties
        dcaegen2_collectors-checkmarx               LICENSE.txt  mvn-phase-lib.sh*  mvn-phase-script.sh*  pom.xml  version.properties
        ccsdk_utils-checkmarx                       platform_base_installation/centos_vm.yaml platform_base_installation/consul.md platform_base_installation/installer platform_base_installation/consul_cluster.yaml platform_base_installation/README.md platform_base_installation/install.md docs/index.rst pom.xml version.properties INFO.yaml
        oparent-checkmarx                           pom.xml only
        ccsdk_parent-checkmarx                      pom.xml only
        ccsdk_platform_blueprints-checkmarx         pom.xml only
        ui-checkmarx                                README.md only
        ncomp-checkmarx                             README.md only
        ncomp_sirius-checkmarx                      README.md only
        aaf_cadi-checkmarx                          SOURCE_MOVED
        aaf_inno-checkmarx                          SOURCE_MOVED
