################################################################################
# Automatically-generated file. Do not edit!
################################################################################

SHELL = cmd.exe

CG_TOOL_ROOT := D:/CCS12.8.1.00005_win64/ccs/tools/compiler/gcc-arm-none-eabi-9-2019-q4-major

GEN_OPTS__FLAG := 
GEN_CMDS__FLAG := 

ORDERED_OBJS += \
"./main_nortos.o" \
"./uart2echo.o" \
"./syscfg/ti_drivers_config.o" \
-Wl,-T"../cc32xxs_nortos.lds" \
$(GEN_CMDS__FLAG) \
-l:ti_utils_build_linker.cmd.genlibs \
-l:"ti/devices/cc32xx/driverlib/gcc/Release/driverlib.a" \
-lgcc \
-lc \
-lm \
-lnosys \

-include ../makefile.init

RM := DEL /F
RMDIR := RMDIR /S/Q

# All of the sources participating in the build are defined here
-include sources.mk
-include subdir_vars.mk
-include subdir_rules.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C55_DEPS)),)
-include $(C55_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(S67_DEPS)),)
-include $(S67_DEPS)
endif
ifneq ($(strip $(S62_DEPS)),)
-include $(S62_DEPS)
endif
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(OPT_DEPS)),)
-include $(OPT_DEPS)
endif
ifneq ($(strip $(C??_DEPS)),)
-include $(C??_DEPS)
endif
ifneq ($(strip $(ASM_UPPER_DEPS)),)
-include $(ASM_UPPER_DEPS)
endif
ifneq ($(strip $(S??_DEPS)),)
-include $(S??_DEPS)
endif
ifneq ($(strip $(C64_DEPS)),)
-include $(C64_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(S64_DEPS)),)
-include $(S64_DEPS)
endif
ifneq ($(strip $(INO_DEPS)),)
-include $(INO_DEPS)
endif
ifneq ($(strip $(CLA_DEPS)),)
-include $(CLA_DEPS)
endif
ifneq ($(strip $(S55_DEPS)),)
-include $(S55_DEPS)
endif
ifneq ($(strip $(SV7A_DEPS)),)
-include $(SV7A_DEPS)
endif
ifneq ($(strip $(C62_DEPS)),)
-include $(C62_DEPS)
endif
ifneq ($(strip $(C67_DEPS)),)
-include $(C67_DEPS)
endif
ifneq ($(strip $(PDE_DEPS)),)
-include $(PDE_DEPS)
endif
ifneq ($(strip $(K_DEPS)),)
-include $(K_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(C43_DEPS)),)
-include $(C43_DEPS)
endif
ifneq ($(strip $(S43_DEPS)),)
-include $(S43_DEPS)
endif
ifneq ($(strip $(ASM_DEPS)),)
-include $(ASM_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
ifneq ($(strip $(SA_DEPS)),)
-include $(SA_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXE_OUTPUTS += \
uart2echo_CC3220S_LAUNCHXL_nortos_gcc.out 

EXE_OUTPUTS__QUOTED += \
"uart2echo_CC3220S_LAUNCHXL_nortos_gcc.out" 

BIN_OUTPUTS += \
uart2echo_CC3220S_LAUNCHXL_nortos_gcc.bin 

BIN_OUTPUTS__QUOTED += \
"uart2echo_CC3220S_LAUNCHXL_nortos_gcc.bin" 

CUSTOM_TOOL_OUTPUTS_701241714 += \
syscfg/uart2echo_CC3220S_LAUNCHXL_nortos_gcc.sli 

CUSTOM_TOOL_OUTPUTS_701241714__QUOTED += \
"syscfg\uart2echo_CC3220S_LAUNCHXL_nortos_gcc.sli" 


# All Target
all: $(OBJS) $(LDS_SRCS) $(GEN_CMDS)
	@$(MAKE) --no-print-directory -Onone "uart2echo_CC3220S_LAUNCHXL_nortos_gcc.out" secondary-outputs

# Tool invocations
uart2echo_CC3220S_LAUNCHXL_nortos_gcc.out: $(OBJS) $(LDS_SRCS) $(GEN_CMDS)
	@echo 'Building target: "$@"'
	@echo 'Invoking: GNU Linker'
	"D:/CCS12.8.1.00005_win64/ccs/tools/compiler/gcc-arm-none-eabi-9-2019-q4-major/bin/arm-none-eabi-gcc-9.2.1.exe" -DDeviceFamily_CC3220 -DNORTOS_SUPPORT -O3 -ffunction-sections -fdata-sections -g -gstrict-dwarf -Wall -march=armv7e-m -mthumb -mfloat-abi=soft -Wl,-Map,"uart2echo_CC3220S_LAUNCHXL_nortos_gcc.map" --entry resetISR -nostartfiles -static -Wl,--gc-sections -L"C:/ti/simplelink_cc32xx_sdk_7_10_00_13/source" -L"C:/ti/simplelink_cc32xx_sdk_7_10_00_13/kernel/nortos" -L"C:/Users/gioan/workspace_v12/uart2echo_CC3220S_LAUNCHXL_nortos_gcc/MCU+Image/syscfg" -L"D:/CCS12.8.1.00005_win64/ccs/tools/compiler/gcc-arm-none-eabi-9-2019-q4-major/arm-none-eabi/lib/thumb/v7e-m/nofp" -march=armv7e-m -mthumb --specs=nano.specs -o"uart2echo_CC3220S_LAUNCHXL_nortos_gcc.out" $(ORDERED_OBJS)
	@echo 'Finished building target: "$@"'
	@echo ' '

uart2echo_CC3220S_LAUNCHXL_nortos_gcc.bin: $(EXE_OUTPUTS)
	@echo 'Building secondary target: "$@"'
	@echo 'Invoking: GNU Objcopy Utility'
	"D:/CCS12.8.1.00005_win64/ccs/tools/compiler/gcc-arm-none-eabi-9-2019-q4-major/bin/arm-none-eabi-objcopy.exe" -O binary $(EXE_OUTPUTS__QUOTED) "uart2echo_CC3220S_LAUNCHXL_nortos_gcc.bin"
	@echo 'Finished building secondary target: "$@"'
	@echo ' '

syscfg/uart2echo_CC3220S_LAUNCHXL_nortos_gcc.sli: $(EXE_OUTPUTS) uart2echo_CC3220S_LAUNCHXL_nortos_gcc.bin syscfg/ti_drivers_net_wifi_config.json
	@echo 'Building secondary target: "$@"'
	@echo 'Invoking: Image Creator'
	"C:/ti/simplelink_cc32xx_sdk_7_10_00_13/source/ti/drivers/net/imagecreator/bin/SLImageCreator.exe" syscfg create_image --sdk_path "C:/ti/simplelink_cc32xx_sdk_7_10_00_13" --json "C:/Users/gioan/workspace_v12/uart2echo_CC3220S_LAUNCHXL_nortos_gcc/MCU+Image/syscfg/ti_drivers_net_wifi_config.json" --file "C:/Users/gioan/workspace_v12/uart2echo_CC3220S_LAUNCHXL_nortos_gcc/MCU+Image/syscfg/uart2echo_CC3220S_LAUNCHXL_nortos_gcc.sli" --mcu "C:/Users/gioan/workspace_v12/uart2echo_CC3220S_LAUNCHXL_nortos_gcc/MCU+Image/uart2echo_CC3220S_LAUNCHXL_nortos_gcc.bin"
	@echo 'Finished building secondary target: "$@"'
	@echo ' '

# Other Targets
clean:
	-$(RM) $(GEN_MISC_FILES__QUOTED)$(BIN_OUTPUTS__QUOTED)$(GEN_FILES__QUOTED)$(CUSTOM_TOOL_OUTPUTS_701241714__QUOTED)$(EXE_OUTPUTS__QUOTED)
	-$(RM) "main_nortos.o" "uart2echo.o" "syscfg\ti_drivers_config.o" 
	-$(RM) "main_nortos.d" "uart2echo.d" "syscfg\ti_drivers_config.d" 
	-$(RMDIR) $(GEN_MISC_DIRS__QUOTED)
	-@echo 'Finished clean'
	-@echo ' '

secondary-outputs: $(BIN_OUTPUTS) $(CUSTOM_TOOL_OUTPUTS_701241714)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets

