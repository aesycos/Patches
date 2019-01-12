## Changed files

kernel/nvidia/nvlink_link.c
kernel/nvidia/os-interface.c
kernel/nvidia-drm/nvidia-drm-connector.c
kernel/nvidia-drm/nvidia-drm-encoder.c
kernel/nvidia-drm/nvidia-drm-gem-nvkms-memory.c
kernel/nvidia-drm/nvidia-drm-gem.h
kernel/nvidia-drm/nvidia-drm-helper.c

## Changes in 5.0.0-rc1

drm_mode_connector_update_edid_property()	=> drm_connector_update_edid_property()

drm_mode_connector_attach_encoder() 		=> drm_connector_attach_encoder()

vm_insert_pfn() 							=> vmf_insert_pfn()

drm_gem_object_unreference_unlocked() 		=> drm_gem_object_put_unlocked()

drm_gem_object_unreference()				=> drm_gem_object_put()

drm_framebuffer_reference() 				=> drm_framebuffer_get()
drm_framebuffer_unreference()				=> drm_framebuffer_put()

drm_dev_unref()								=> drm_dev_put()
drm_dev_free()

void do_gettimeofday(struct timeval *tv)		// in <include/linux/timekeeping32.h> as of 4.15-rc1
												// in <include/linux/timekeeping.h>

void efi_gettimeofday(struct timespec64 *ts)	// in <include/efi.h> as of 4.8-rc1
