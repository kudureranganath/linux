# SPDX-License-Identifier: GPL-2.0
#
# Makefile for the linux ppc-specific parts of the memory manager.
#

obj-y				:= fault.o mem.o pgtable.o maccess.o pageattr.o \
				   init_$(BITS).o pgtable_$(BITS).o \
				   pgtable-frag.o ioremap.o ioremap_$(BITS).o \
				   init-common.o mmu_context.o drmem.o \
				   cacheflush.o
obj-$(CONFIG_PPC_MMU_NOHASH)	+= nohash/
obj-$(CONFIG_PPC_BOOK3S_32)	+= book3s32/
obj-$(CONFIG_PPC_BOOK3S_64)	+= book3s64/
obj-$(CONFIG_NUMA) += numa.o
obj-$(CONFIG_HUGETLB_PAGE)	+= hugetlbpage.o
obj-$(CONFIG_NOT_COHERENT_CACHE) += dma-noncoherent.o
obj-$(CONFIG_PPC_COPRO_BASE)	+= copro_fault.o
obj-$(CONFIG_PTDUMP)		+= ptdump/
obj-$(CONFIG_KASAN)		+= kasan/
