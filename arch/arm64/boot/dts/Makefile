dtb-$(CONFIG_MACH_EXYNOS7880_A5Y17LTE_CAN_OPEN) := \
	exynos7880-a5y17lte_can_open_00.dtb \
	exynos7880-a5y17lte_can_open_01.dtb \
	exynos7880-a5y17lte_can_open_02.dtb \
	exynos7880-a5y17lte_can_open_03.dtb \
	exynos7880-a5y17lte_can_open_05.dtb \
	exynos7880-a5y17lte_can_open_07.dtb \
	exynos7880-a5y17lte_can_open_08.dtb
dtb-$(CONFIG_MACH_EXYNOS7880_A5Y17LTE_EUR_LDU) := \
	exynos7880-a5y17lte_eur_ldu_00.dtb \
	exynos7880-a5y17lte_eur_ldu_01.dtb \
	exynos7880-a5y17lte_eur_ldu_02.dtb \
	exynos7880-a5y17lte_eur_ldu_03.dtb \
	exynos7880-a5y17lte_eur_ldu_05.dtb \
	exynos7880-a5y17lte_eur_ldu_07.dtb \
	exynos7880-a5y17lte_eur_ldu_08.dtb
dtb-$(CONFIG_MACH_EXYNOS7880_A5Y17LTE_EUR_OPEN) := \
	exynos7880-a5y17lte_eur_open_00.dtb \
	exynos7880-a5y17lte_eur_open_01.dtb \
	exynos7880-a5y17lte_eur_open_02.dtb \
	exynos7880-a5y17lte_eur_open_03.dtb \
	exynos7880-a5y17lte_eur_open_05.dtb \
	exynos7880-a5y17lte_eur_open_07.dtb \
	exynos7880-a5y17lte_eur_open_08.dtb
dtb-$(CONFIG_MACH_EXYNOS7880_A5Y17LTE_KOR_ALL) := \
	exynos7880-a5y17lte_kor_all_00.dtb \
	exynos7880-a5y17lte_kor_all_01.dtb \
	exynos7880-a5y17lte_kor_all_02.dtb \
	exynos7880-a5y17lte_kor_all_03.dtb \
	exynos7880-a5y17lte_kor_all_05.dtb \
	exynos7880-a5y17lte_kor_all_07.dtb \
	exynos7880-a5y17lte_kor_all_08.dtb \
	exynos7880-a5y17lte_kor_all_09.dtb
dtb-$(CONFIG_MACH_EXYNOS7880_A7Y17LTE_EUR_LDU) := \
	exynos7880-a7y17lte_eur_ldu_00.dtb \
	exynos7880-a7y17lte_eur_ldu_01.dtb \
	exynos7880-a7y17lte_eur_ldu_02.dtb \
	exynos7880-a7y17lte_eur_ldu_03.dtb \
	exynos7880-a7y17lte_eur_ldu_04.dtb \
	exynos7880-a7y17lte_eur_ldu_06.dtb
dtb-$(CONFIG_MACH_EXYNOS7880_A7Y17LTE_EUR_OPEN) := \
	exynos7880-a7y17lte_eur_open_00.dtb \
	exynos7880-a7y17lte_eur_open_01.dtb \
	exynos7880-a7y17lte_eur_open_02.dtb \
	exynos7880-a7y17lte_eur_open_03.dtb \
	exynos7880-a7y17lte_eur_open_04.dtb \
	exynos7880-a7y17lte_eur_open_06.dtb
dtb-$(CONFIG_MACH_EXYNOS7880_A7Y17LTE_KOR_ALL) := \
	exynos7880-a7y17lte_kor_all_00.dtb \
	exynos7880-a7y17lte_kor_all_01.dtb \
	exynos7880-a7y17lte_kor_all_02.dtb \
	exynos7880-a7y17lte_kor_all_03.dtb \
	exynos7880-a7y17lte_kor_all_04.dtb \
	exynos7880-a7y17lte_kor_all_06.dtb

targets += dtbs

DTB_NAMES := $(subst $\",,$(CONFIG_BUILD_ARM64_APPENDED_DTB_IMAGE_NAMES))
ifneq ($(DTB_NAMES),)
DTB_LIST := $(addsuffix .dtb,$(DTB_NAMES))
else
DTB_LIST := $(dtb-y)
endif
targets += $(DTB_LIST)

dtbs: $(addprefix $(obj)/, $(DTB_LIST))

clean-files := dts/*.dtb *.dtb
