idf_component_register(SRCS "azure_main.c" "custom_hsm_x509.c" "prov_dev_client_ll_sample.c"
                       INCLUDE_DIRS "."
                       EMBED_TXTFILES "certs/leaf_certificate.pem" "certs/leaf_private_key.pem")

target_compile_definitions(${COMPONENT_LIB} PRIVATE SET_TRUSTED_CERT_IN_SAMPLES)
