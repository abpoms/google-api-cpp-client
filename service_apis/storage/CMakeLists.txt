# This is a CMake file for Cloud Storage JSON API v1
# using the Google APIs Client Library for C++.
#
# See http://google.github.io/google-api-cpp-client/latest/start/get_started
# for more information about what to do with this file.

project (storage)
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/.)

add_subdirectory(google/storage_api)

install(FILES google/storage_api/bucket_access_control.h
	      google/storage_api/object_access_control.h
	      google/storage_api/bucket.h
	      google/storage_api/bucket_access_controls.h
	      google/storage_api/buckets.h
	      google/storage_api/channel.h
	      google/storage_api/object.h
	      google/storage_api/compose_request.h
	      google/storage_api/object_access_controls.h
	      google/storage_api/objects.h
	      google/storage_api/rewrite_response.h
	      google/storage_api/storage_service.h
	      google/storage_api/storage_api.h
        DESTINATION ${GOOGLEAPIS_INSTALL_INCLUDE_DIR}/../google/storage_api)
