idf_component_register(SRCS "azure_main.c" "iothub_client_device_twin_and_methods_sample.c"
                       INCLUDE_DIRS ".")

target_compile_definitions(${COMPONENT_LIB} PRIVATE SET_TRUSTED_CERT_IN_SAMPLES)
