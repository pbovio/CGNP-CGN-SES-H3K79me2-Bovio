# CGNP-CGN-SES-H3K79me2-Bovio
{
    "a_galaxy_workflow": "true", 
    "annotation": "", 
    "format-version": "0.1", 
    "name": "CGNP/CGN for comparable ChIPseq H3K79me2", 
    "steps": {
        "0": {
            "annotation": "", 
            "content_id": null, 
            "id": 0, 
            "input_connections": {}, 
            "inputs": [
                {
                    "description": "", 
                    "name": "ChIP-CGN-UT-R1"
                }
            ], 
            "label": null, 
            "name": "Input dataset", 
            "outputs": [], 
            "position": {
                "left": 231.08331298828125, 
                "top": 507.88330078125
            }, 
            "tool_errors": null, 
            "tool_id": null, 
            "tool_state": "{\"name\": \"ChIP-CGN-UT-R1\"}", 
            "tool_version": null, 
            "type": "data_input", 
            "uuid": "None", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "63fec1fb-e672-474a-9c9e-7c84b82d1910"
                }
            ]
        }, 
        "1": {
            "annotation": "", 
            "content_id": null, 
            "id": 1, 
            "input_connections": {}, 
            "inputs": [
                {
                    "description": "", 
                    "name": "ChIP-CGN-UT-R2"
                }
            ], 
            "label": null, 
            "name": "Input dataset", 
            "outputs": [], 
            "position": {
                "left": 230, 
                "top": 567.7166748046875
            }, 
            "tool_errors": null, 
            "tool_id": null, 
            "tool_state": "{\"name\": \"ChIP-CGN-UT-R2\"}", 
            "tool_version": null, 
            "type": "data_input", 
            "uuid": "bfcbc824-3653-46b9-9870-3e0b5bf5cbec", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "6f0602c1-66c5-4a83-8b7b-a6e16339d573"
                }
            ]
        }, 
        "2": {
            "annotation": "", 
            "content_id": null, 
            "id": 2, 
            "input_connections": {}, 
            "inputs": [
                {
                    "description": "", 
                    "name": "Input-CGN-UT-R1"
                }
            ], 
            "label": null, 
            "name": "Input dataset", 
            "outputs": [], 
            "position": {
                "left": 239.08331298828125, 
                "top": 997.88330078125
            }, 
            "tool_errors": null, 
            "tool_id": null, 
            "tool_state": "{\"name\": \"Input-CGN-UT-R1\"}", 
            "tool_version": null, 
            "type": "data_input", 
            "uuid": "None", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "da5158f0-a806-47da-a452-3e7b4388744c"
                }
            ]
        }, 
        "3": {
            "annotation": "", 
            "content_id": null, 
            "id": 3, 
            "input_connections": {}, 
            "inputs": [
                {
                    "description": "", 
                    "name": "Input-CGN-UT-R2"
                }
            ], 
            "label": null, 
            "name": "Input dataset", 
            "outputs": [], 
            "position": {
                "left": 236, 
                "top": 1050.7166748046875
            }, 
            "tool_errors": null, 
            "tool_id": null, 
            "tool_state": "{\"name\": \"Input-CGN-UT-R2\"}", 
            "tool_version": null, 
            "type": "data_input", 
            "uuid": "4cb0bcc3-9913-487d-af57-c5736b7ae7ec", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "678c48a8-2721-4607-9d96-9ba5637393af"
                }
            ]
        }, 
        "4": {
            "annotation": "", 
            "content_id": null, 
            "id": 4, 
            "input_connections": {}, 
            "inputs": [
                {
                    "description": "", 
                    "name": "UCSC mm10 refGen.bed"
                }
            ], 
            "label": null, 
            "name": "Input dataset", 
            "outputs": [], 
            "position": {
                "left": 1718.0833740234375, 
                "top": 1546.88330078125
            }, 
            "tool_errors": null, 
            "tool_id": null, 
            "tool_state": "{\"name\": \"UCSC mm10 refGen.bed\"}", 
            "tool_version": null, 
            "type": "data_input", 
            "uuid": "None", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "69e7fb2c-f70f-4bf6-81ef-61965affa027"
                }
            ]
        }, 
        "5": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "id": 5, 
            "input_connections": {
                "input_file": {
                    "id": 0, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "contaminants"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "limits"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "input_file"
                }
            ], 
            "label": null, 
            "name": "FastQC", 
            "outputs": [
                {
                    "name": "html_file", 
                    "type": "html"
                }, 
                {
                    "name": "text_file", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 436.25, 
                "top": 352.75
            }, 
            "post_job_actions": {
                "HideDatasetActiontext_file": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "text_file"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "tool_shed_repository": {
                "changeset_revision": "3fdc1a74d866", 
                "name": "fastqc", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"contaminants\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__rerun_remap_job_id__\": null, \"limits\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"input_file\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "0.65", 
            "type": "tool", 
            "uuid": "d8ed7cf0-37e5-4268-a484-3bd5d4f0e51a", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "html_file", 
                    "uuid": "6e8d6205-7347-4bd8-9ff1-5b67f5c3719d"
                }
            ]
        }, 
        "6": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "id": 6, 
            "input_connections": {
                "input_file": {
                    "id": 1, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "contaminants"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "limits"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "input_file"
                }
            ], 
            "label": null, 
            "name": "FastQC", 
            "outputs": [
                {
                    "name": "html_file", 
                    "type": "html"
                }, 
                {
                    "name": "text_file", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 432.25, 
                "top": 583.75
            }, 
            "post_job_actions": {
                "HideDatasetActiontext_file": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "text_file"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "tool_shed_repository": {
                "changeset_revision": "3fdc1a74d866", 
                "name": "fastqc", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"contaminants\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__rerun_remap_job_id__\": null, \"limits\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"input_file\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "0.65", 
            "type": "tool", 
            "uuid": "f7cbd853-ff19-4d70-bc79-0cae6fdbd701", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "html_file", 
                    "uuid": "401906de-1786-444f-bafa-150719f1f00b"
                }
            ]
        }, 
        "7": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/bowtie2/bowtie2/2.2.6.2", 
            "id": 7, 
            "input_connections": {
                "library|input_1": {
                    "id": 0, 
                    "output_name": "output"
                }, 
                "library|input_2": {
                    "id": 1, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool Bowtie2", 
                    "name": "library"
                }, 
                {
                    "description": "runtime parameter for tool Bowtie2", 
                    "name": "library"
                }
            ], 
            "label": null, 
            "name": "Bowtie2", 
            "outputs": [
                {
                    "name": "output_unaligned_reads_l", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output_aligned_reads_l", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output_aligned_reads_r", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output_unaligned_reads_r", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output", 
                    "type": "bam"
                }, 
                {
                    "name": "output_sam", 
                    "type": "sam"
                }, 
                {
                    "name": "mapping_stats", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 765.25, 
                "top": 416.75
            }, 
            "post_job_actions": {
                "HideDatasetActionmapping_stats": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "mapping_stats"
                }, 
                "HideDatasetActionoutput_aligned_reads_l": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_aligned_reads_l"
                }, 
                "HideDatasetActionoutput_aligned_reads_r": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_aligned_reads_r"
                }, 
                "HideDatasetActionoutput_sam": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_sam"
                }, 
                "HideDatasetActionoutput_unaligned_reads_l": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_unaligned_reads_l"
                }, 
                "HideDatasetActionoutput_unaligned_reads_r": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_unaligned_reads_r"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/bowtie2/bowtie2/2.2.6.2", 
            "tool_shed_repository": {
                "changeset_revision": "a9d4f71dbfb0", 
                "name": "bowtie2", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"library\": \"{\\\"aligned_file\\\": \\\"false\\\", \\\"unaligned_file\\\": \\\"false\\\", \\\"input_2\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}, \\\"__current_case__\\\": 1, \\\"input_1\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}, \\\"type\\\": \\\"paired\\\", \\\"paired_options\\\": {\\\"paired_options_selector\\\": \\\"no\\\", \\\"__current_case__\\\": 1}}\", \"reference_genome\": \"{\\\"source\\\": \\\"indexed\\\", \\\"__current_case__\\\": 0, \\\"index\\\": \\\"mm10\\\"}\", \"rg\": \"{\\\"rg_selector\\\": \\\"do_not_set\\\", \\\"__current_case__\\\": 3}\", \"save_mapping_stats\": \"\\\"false\\\"\", \"analysis_type\": \"{\\\"analysis_type_selector\\\": \\\"simple\\\", \\\"presets\\\": \\\"no_presets\\\", \\\"__current_case__\\\": 0}\"}", 
            "tool_version": "2.2.6.2", 
            "type": "tool", 
            "uuid": "2945f135-b70d-4e4c-babc-b6dd1711d19c", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "47c9502d-1b2f-4ebe-90be-f0f94732ce79"
                }
            ]
        }, 
        "8": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "id": 8, 
            "input_connections": {
                "input_file": {
                    "id": 2, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "contaminants"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "limits"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "input_file"
                }
            ], 
            "label": null, 
            "name": "FastQC", 
            "outputs": [
                {
                    "name": "html_file", 
                    "type": "html"
                }, 
                {
                    "name": "text_file", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 436.25, 
                "top": 843.75
            }, 
            "post_job_actions": {
                "HideDatasetActiontext_file": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "text_file"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "tool_shed_repository": {
                "changeset_revision": "3fdc1a74d866", 
                "name": "fastqc", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"contaminants\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__rerun_remap_job_id__\": null, \"limits\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"input_file\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "0.65", 
            "type": "tool", 
            "uuid": "a18f93d7-06cf-4724-9eba-a001386a1a79", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "html_file", 
                    "uuid": "206997d6-3be0-4b4c-ba5e-f7c3eea5ef38"
                }
            ]
        }, 
        "9": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "id": 9, 
            "input_connections": {
                "input_file": {
                    "id": 3, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "contaminants"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "limits"
                }, 
                {
                    "description": "runtime parameter for tool FastQC", 
                    "name": "input_file"
                }
            ], 
            "label": null, 
            "name": "FastQC", 
            "outputs": [
                {
                    "name": "html_file", 
                    "type": "html"
                }, 
                {
                    "name": "text_file", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 434.25, 
                "top": 1075.75
            }, 
            "post_job_actions": {
                "HideDatasetActiontext_file": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "text_file"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/fastqc/fastqc/0.65", 
            "tool_shed_repository": {
                "changeset_revision": "3fdc1a74d866", 
                "name": "fastqc", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"contaminants\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__rerun_remap_job_id__\": null, \"limits\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"input_file\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "0.65", 
            "type": "tool", 
            "uuid": "7dbe59d0-7d88-44a9-9bc9-c45123c2d9aa", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "html_file", 
                    "uuid": "8172cfbe-e745-4ef7-ae88-51ddb7cea7e9"
                }
            ]
        }, 
        "10": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/bowtie2/bowtie2/2.2.6.2", 
            "id": 10, 
            "input_connections": {
                "library|input_1": {
                    "id": 2, 
                    "output_name": "output"
                }, 
                "library|input_2": {
                    "id": 3, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool Bowtie2", 
                    "name": "library"
                }, 
                {
                    "description": "runtime parameter for tool Bowtie2", 
                    "name": "library"
                }
            ], 
            "label": null, 
            "name": "Bowtie2", 
            "outputs": [
                {
                    "name": "output_unaligned_reads_l", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output_aligned_reads_l", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output_aligned_reads_r", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output_unaligned_reads_r", 
                    "type": "fastqsanger"
                }, 
                {
                    "name": "output", 
                    "type": "bam"
                }, 
                {
                    "name": "output_sam", 
                    "type": "sam"
                }, 
                {
                    "name": "mapping_stats", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 762.25, 
                "top": 995.75
            }, 
            "post_job_actions": {
                "HideDatasetActionmapping_stats": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "mapping_stats"
                }, 
                "HideDatasetActionoutput_aligned_reads_l": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_aligned_reads_l"
                }, 
                "HideDatasetActionoutput_aligned_reads_r": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_aligned_reads_r"
                }, 
                "HideDatasetActionoutput_unaligned_reads_l": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_unaligned_reads_l"
                }, 
                "HideDatasetActionoutput_unaligned_reads_r": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_unaligned_reads_r"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/bowtie2/bowtie2/2.2.6.2", 
            "tool_shed_repository": {
                "changeset_revision": "a9d4f71dbfb0", 
                "name": "bowtie2", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"library\": \"{\\\"aligned_file\\\": \\\"false\\\", \\\"unaligned_file\\\": \\\"false\\\", \\\"input_2\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}, \\\"__current_case__\\\": 1, \\\"input_1\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}, \\\"type\\\": \\\"paired\\\", \\\"paired_options\\\": {\\\"paired_options_selector\\\": \\\"no\\\", \\\"__current_case__\\\": 1}}\", \"reference_genome\": \"{\\\"source\\\": \\\"indexed\\\", \\\"__current_case__\\\": 0, \\\"index\\\": \\\"mm10\\\"}\", \"rg\": \"{\\\"rg_selector\\\": \\\"do_not_set\\\", \\\"__current_case__\\\": 3}\", \"save_mapping_stats\": \"\\\"false\\\"\", \"analysis_type\": \"{\\\"analysis_type_selector\\\": \\\"simple\\\", \\\"presets\\\": \\\"no_presets\\\", \\\"__current_case__\\\": 0}\"}", 
            "tool_version": "2.2.6.2", 
            "type": "tool", 
            "uuid": "d69bcefa-8068-4e19-91c1-5ddd7c50f915", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output", 
                    "uuid": "279ecd85-9e80-4dbe-b848-c4f5f2f5f0e7"
                }, 
                {
                    "label": null, 
                    "output_name": "output_sam", 
                    "uuid": "45d631a0-b30c-4d4a-884e-71a263bd1457"
                }
            ]
        }, 
        "11": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_sort/samtools_sort/2.0", 
            "id": 11, 
            "input_connections": {
                "input1": {
                    "id": 7, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool Sort", 
                    "name": "input1"
                }
            ], 
            "label": null, 
            "name": "Sort", 
            "outputs": [
                {
                    "name": "output1", 
                    "type": "bam"
                }
            ], 
            "position": {
                "left": 864.8333740234375, 
                "top": 247.5
            }, 
            "post_job_actions": {}, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_sort/samtools_sort/2.0", 
            "tool_shed_repository": {
                "changeset_revision": "a430da4f04cd", 
                "name": "samtools_sort", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"input1\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"sort_mode\": \"\\\"\\\"\"}", 
            "tool_version": "2.0", 
            "type": "tool", 
            "uuid": "f11c28b4-9437-4a81-aafb-10e39560c8f4", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output1", 
                    "uuid": "35212751-bc3e-4890-929c-c1cb26b99262"
                }
            ]
        }, 
        "12": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_CollectInsertSizeMetrics/1.136.0", 
            "id": 12, 
            "input_connections": {
                "inputFile": {
                    "id": 7, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool CollectInsertSizeMetrics", 
                    "name": "inputFile"
                }
            ], 
            "label": null, 
            "name": "CollectInsertSizeMetrics", 
            "outputs": [
                {
                    "name": "outFile", 
                    "type": "tabular"
                }, 
                {
                    "name": "histFile", 
                    "type": "pdf"
                }
            ], 
            "position": {
                "left": 1169.63330078125, 
                "top": 338.29998779296875
            }, 
            "post_job_actions": {}, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_CollectInsertSizeMetrics/1.136.0", 
            "tool_shed_repository": {
                "changeset_revision": "efc56ee1ade4", 
                "name": "picard", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"deviations\": \"\\\"10.0\\\"\", \"__rerun_remap_job_id__\": null, \"hist_width\": \"\\\"\\\"\", \"assume_sorted\": \"\\\"true\\\"\", \"metric_accumulation_level\": \"[\\\"ALL_READS\\\"]\", \"validation_stringency\": \"\\\"LENIENT\\\"\", \"reference_source\": \"{\\\"ref_file\\\": \\\"mm10full\\\", \\\"reference_source_selector\\\": \\\"cached\\\", \\\"__current_case__\\\": 0}\", \"min_pct\": \"\\\"0.05\\\"\", \"inputFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "1.136.0", 
            "type": "tool", 
            "uuid": "b2df503a-d632-47ae-a68d-1fe5870058f1", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFile", 
                    "uuid": "21b0b1fa-6d6e-432f-81da-4c79f62a54ed"
                }, 
                {
                    "label": null, 
                    "output_name": "histFile", 
                    "uuid": "d056ea31-66fc-44f3-a3b1-03e6b40cb6fd"
                }
            ]
        }, 
        "13": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_gc_bias/deeptools_compute_gc_bias/2.2.3.0", 
            "id": 13, 
            "input_connections": {
                "bamInput": {
                    "id": 7, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool computeGCBias", 
                    "name": "bamInput"
                }, 
                {
                    "description": "runtime parameter for tool computeGCBias", 
                    "name": "advancedOpt"
                }, 
                {
                    "description": "runtime parameter for tool computeGCBias", 
                    "name": "advancedOpt"
                }
            ], 
            "label": null, 
            "name": "computeGCBias", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "tabular"
                }, 
                {
                    "name": "outImageName", 
                    "type": "png"
                }
            ], 
            "position": {
                "left": 1172.183349609375, 
                "top": 472.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileName": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileName"
                }, 
                "HideDatasetActionoutImageName": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outImageName"
                }, 
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "ChIP-CGN-UT"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_gc_bias/deeptools_compute_gc_bias/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "6a056fb2b9c1", 
                "name": "deeptools_compute_gc_bias", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"region\": \"\\\"\\\"\", \"bamInput\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"source\": \"{\\\"input1_2bit\\\": \\\"mm10\\\", \\\"ref_source\\\": \\\"cached\\\", \\\"__current_case__\\\": 0}\", \"__rerun_remap_job_id__\": null, \"effectiveGenomeSize\": \"{\\\"effectiveGenomeSize_opt\\\": \\\"2150570000\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"filterOut\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}, \\\"extraSampling\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}, \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"sampleSize\\\": \\\"50000000\\\", \\\"__current_case__\\\": 1, \\\"regionSize\\\": \\\"300\\\"}\", \"image_format\": \"\\\"png\\\"\", \"fragmentLength\": \"\\\"300\\\"\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "e8fce3ae-7e11-47fd-833c-453b78f6ab42", 
            "workflow_outputs": []
        }, 
        "14": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_flagstat/samtools_flagstat/2.0", 
            "id": 14, 
            "input_connections": {
                "input1": {
                    "id": 7, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool Flagstat", 
                    "name": "input1"
                }
            ], 
            "label": null, 
            "name": "Flagstat", 
            "outputs": [
                {
                    "name": "output1", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 1172.949951171875, 
                "top": 726.5166625976562
            }, 
            "post_job_actions": {
                "HideDatasetActionoutput1": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output1"
                }, 
                "TagDatasetActionoutput1": {
                    "action_arguments": {
                        "tags": "ChIP-CGN-UT"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "output1"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_flagstat/samtools_flagstat/2.0", 
            "tool_shed_repository": {
                "changeset_revision": "0072bf593791", 
                "name": "samtools_flagstat", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"input1\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.0", 
            "type": "tool", 
            "uuid": "bc8e8c0e-8747-496b-ab11-30853fee845e", 
            "workflow_outputs": []
        }, 
        "15": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_multi_bam_summary/deeptools_multi_bam_summary/2.2.3.0", 
            "id": 15, 
            "input_connections": {
                "bamfiles": [
                    {
                        "id": 10, 
                        "output_name": "output"
                    }, 
                    {
                        "id": 7, 
                        "output_name": "output"
                    }
                ]
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool multiBamSummary", 
                    "name": "bamfiles"
                }
            ], 
            "label": null, 
            "name": "multiBamSummary", 
            "outputs": [
                {
                    "name": "outFile", 
                    "type": "deeptools_coverage_matrix"
                }, 
                {
                    "name": "outFileRawCounts", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 1092.4166259765625, 
                "top": 838.4166870117188
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileRawCounts": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileRawCounts"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_multi_bam_summary/deeptools_multi_bam_summary/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "87d2c75884d9", 
                "name": "deeptools_multi_bam_summary", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"bamfiles\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"region\": \"\\\"\\\"\", \"mode\": \"{\\\"binSize\\\": \\\"10000\\\", \\\"distanceBetweenBins\\\": \\\"10000\\\", \\\"__current_case__\\\": 0, \\\"modeOpt\\\": \\\"bins\\\"}\", \"advancedOpt\": \"{\\\"ignoreDuplicates\\\": \\\"false\\\", \\\"centerReads\\\": \\\"false\\\", \\\"doExtendCustom\\\": {\\\"__current_case__\\\": 0, \\\"doExtend\\\": \\\"no\\\"}, \\\"samFlagExclude\\\": \\\"\\\", \\\"samFlagInclude\\\": \\\"\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"minMappingQuality\\\": \\\"1\\\"}\", \"__rerun_remap_job_id__\": null, \"outRawCounts\": \"\\\"false\\\"\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "6f537383-7dea-4bdd-a408-31c7041618c8", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFile", 
                    "uuid": "2e4619e1-e878-4ff2-a41b-da3319f53745"
                }
            ]
        }, 
        "16": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_flagstat/samtools_flagstat/2.0", 
            "id": 16, 
            "input_connections": {
                "input1": {
                    "id": 10, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool Flagstat", 
                    "name": "input1"
                }
            ], 
            "label": null, 
            "name": "Flagstat", 
            "outputs": [
                {
                    "name": "output1", 
                    "type": "txt"
                }
            ], 
            "position": {
                "left": 1171.949951171875, 
                "top": 1058.5166015625
            }, 
            "post_job_actions": {
                "HideDatasetActionoutput1": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output1"
                }, 
                "TagDatasetActionoutput1": {
                    "action_arguments": {
                        "tags": "ChIP-CGN-UT"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "output1"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_flagstat/samtools_flagstat/2.0", 
            "tool_shed_repository": {
                "changeset_revision": "0072bf593791", 
                "name": "samtools_flagstat", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"input1\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.0", 
            "type": "tool", 
            "uuid": "bdebbcd4-b7ae-4fed-8c64-43f1b1260b74", 
            "workflow_outputs": []
        }, 
        "17": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_sort/samtools_sort/2.0", 
            "id": 17, 
            "input_connections": {
                "input1": {
                    "id": 10, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool Sort", 
                    "name": "input1"
                }
            ], 
            "label": null, 
            "name": "Sort", 
            "outputs": [
                {
                    "name": "output1", 
                    "type": "bam"
                }
            ], 
            "position": {
                "left": 848.8333740234375, 
                "top": 1403.5
            }, 
            "post_job_actions": {}, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/samtools_sort/samtools_sort/2.0", 
            "tool_shed_repository": {
                "changeset_revision": "a430da4f04cd", 
                "name": "samtools_sort", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"input1\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"sort_mode\": \"\\\"\\\"\"}", 
            "tool_version": "2.0", 
            "type": "tool", 
            "uuid": "e9ff5b7e-2973-4069-a264-8aaa974c0bbc", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output1", 
                    "uuid": "f49cdc6b-ce27-48ca-bd07-87de53ac9caf"
                }
            ]
        }, 
        "18": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_gc_bias/deeptools_compute_gc_bias/2.2.3.0", 
            "id": 18, 
            "input_connections": {
                "bamInput": {
                    "id": 10, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool computeGCBias", 
                    "name": "bamInput"
                }
            ], 
            "label": null, 
            "name": "computeGCBias", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "tabular"
                }, 
                {
                    "name": "outImageName", 
                    "type": "png"
                }
            ], 
            "position": {
                "left": 1169.183349609375, 
                "top": 1151.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileName": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileName"
                }, 
                "HideDatasetActionoutImageName": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outImageName"
                }, 
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "Input-CGN-UT"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_gc_bias/deeptools_compute_gc_bias/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "6a056fb2b9c1", 
                "name": "deeptools_compute_gc_bias", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"region\": \"\\\"\\\"\", \"bamInput\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"source\": \"{\\\"input1_2bit\\\": \\\"mm10\\\", \\\"ref_source\\\": \\\"cached\\\", \\\"__current_case__\\\": 0}\", \"__rerun_remap_job_id__\": null, \"effectiveGenomeSize\": \"{\\\"effectiveGenomeSize_opt\\\": \\\"2150570000\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"showAdvancedOpt\\\": \\\"no\\\", \\\"__current_case__\\\": 0}\", \"image_format\": \"\\\"png\\\"\", \"fragmentLength\": \"\\\"300\\\"\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "aa56ad49-d05a-4a07-b79a-70d9f9455ce3", 
            "workflow_outputs": []
        }, 
        "19": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_CollectInsertSizeMetrics/1.136.0", 
            "id": 19, 
            "input_connections": {
                "inputFile": {
                    "id": 10, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool CollectInsertSizeMetrics", 
                    "name": "inputFile"
                }
            ], 
            "label": null, 
            "name": "CollectInsertSizeMetrics", 
            "outputs": [
                {
                    "name": "outFile", 
                    "type": "tabular"
                }, 
                {
                    "name": "histFile", 
                    "type": "pdf"
                }
            ], 
            "position": {
                "left": 1166.3333740234375, 
                "top": 1401.5
            }, 
            "post_job_actions": {}, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_CollectInsertSizeMetrics/1.136.0", 
            "tool_shed_repository": {
                "changeset_revision": "efc56ee1ade4", 
                "name": "picard", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"deviations\": \"\\\"10.0\\\"\", \"__rerun_remap_job_id__\": null, \"hist_width\": \"\\\"\\\"\", \"assume_sorted\": \"\\\"true\\\"\", \"metric_accumulation_level\": \"[\\\"ALL_READS\\\"]\", \"validation_stringency\": \"\\\"LENIENT\\\"\", \"reference_source\": \"{\\\"ref_file\\\": \\\"mm10full\\\", \\\"reference_source_selector\\\": \\\"cached\\\", \\\"__current_case__\\\": 0}\", \"min_pct\": \"\\\"0.05\\\"\", \"inputFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "1.136.0", 
            "type": "tool", 
            "uuid": "d448f240-a407-4412-a739-0c271aaaba5a", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFile", 
                    "uuid": "35ef8ecc-6df1-4d40-9ad8-731a560a45bc"
                }, 
                {
                    "label": null, 
                    "output_name": "histFile", 
                    "uuid": "cf727c5a-49f2-41a9-940c-3463bc31f81b"
                }
            ]
        }, 
        "20": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_MarkDuplicates/1.136.0", 
            "id": 20, 
            "input_connections": {
                "inputFile": {
                    "id": 11, 
                    "output_name": "output1"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool MarkDuplicates", 
                    "name": "inputFile"
                }
            ], 
            "label": null, 
            "name": "MarkDuplicates", 
            "outputs": [
                {
                    "name": "metrics_file", 
                    "type": "txt"
                }, 
                {
                    "name": "outFile", 
                    "type": "bam"
                }
            ], 
            "position": {
                "left": 1170.5833740234375, 
                "top": 202
            }, 
            "post_job_actions": {
                "HideDatasetActionmetrics_file": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "metrics_file"
                }, 
                "TagDatasetActionmetrics_file": {
                    "action_arguments": {
                        "tags": "ChIP-CGN-UT-rmdup"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "metrics_file"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_MarkDuplicates/1.136.0", 
            "tool_shed_repository": {
                "changeset_revision": "efc56ee1ade4", 
                "name": "picard", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"duplicate_scoring_strategy\": \"\\\"SUM_OF_BASE_QUALITIES\\\"\", \"remove_duplicates\": \"\\\"true\\\"\", \"read_name_regex\": \"\\\"[a-zA-Z0-9]+:[0-9]:([0-9]+):([0-9]+):([0-9]+).*.\\\"\", \"__page__\": 0, \"__rerun_remap_job_id__\": null, \"optical_duplicate_pixel_distance\": \"\\\"100\\\"\", \"comments\": \"[]\", \"assume_sorted\": \"\\\"true\\\"\", \"validation_stringency\": \"\\\"LENIENT\\\"\", \"inputFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "1.136.0", 
            "type": "tool", 
            "uuid": "ad536ac4-8396-46b6-9cb7-8f73088ad9d9", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFile", 
                    "uuid": "430ae35f-7366-4478-ab84-6bc7eef1ad68"
                }
            ]
        }, 
        "21": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_correlation/deeptools_plot_correlation/2.2.3.0", 
            "id": 21, 
            "input_connections": {
                "corData": {
                    "id": 15, 
                    "output_name": "outFile"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool plotCorrelation", 
                    "name": "corData"
                }
            ], 
            "label": null, 
            "name": "plotCorrelation", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "png"
                }, 
                {
                    "name": "matrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 1392.183349609375, 
                "top": 858.75
            }, 
            "post_job_actions": {
                "HideDatasetActionmatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "matrix"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_correlation/deeptools_plot_correlation/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "b3589208f673", 
                "name": "deeptools_plot_correlation", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"removeOutliers\": \"\\\"false\\\"\", \"outFileFormat\": \"\\\"png\\\"\", \"outFileCorMatrix\": \"\\\"false\\\"\", \"__rerun_remap_job_id__\": null, \"corMethod\": \"\\\"pearson\\\"\", \"skipZeros\": \"\\\"false\\\"\", \"plotting_type\": \"{\\\"plotTitle\\\": \\\"\\\", \\\"colorMap\\\": \\\"RdYlBu\\\", \\\"plotNumbers\\\": \\\"false\\\", \\\"zMin\\\": \\\"\\\", \\\"whatToPlot\\\": \\\"heatmap\\\", \\\"__current_case__\\\": 0, \\\"zMax\\\": \\\"\\\"}\", \"corData\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "efb201a6-e6a0-44e3-87fd-dbe7e9cac938", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "7a9af483-d54f-4c91-b444-4a6f51d18ca3"
                }
            ]
        }, 
        "22": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_fingerprint/deeptools_plot_fingerprint/2.2.3.0", 
            "id": 22, 
            "input_connections": {
                "bamfiles": [
                    {
                        "id": 17, 
                        "output_name": "output1"
                    }, 
                    {
                        "id": 11, 
                        "output_name": "output1"
                    }
                ]
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool plotFingerprint", 
                    "name": "bamfiles"
                }
            ], 
            "label": null, 
            "name": "plotFingerprint", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "png"
                }, 
                {
                    "name": "outFileRawCounts", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 782.25, 
                "top": 801.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileName": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileName"
                }, 
                "HideDatasetActionoutFileRawCounts": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileRawCounts"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_fingerprint/deeptools_plot_fingerprint/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "e94df7973bb0", 
                "name": "deeptools_plot_fingerprint", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"bamfiles\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__rerun_remap_job_id__\": null, \"output\": \"{\\\"showOutputSettings\\\": \\\"no\\\", \\\"__current_case__\\\": 0}\", \"advancedOpt\": \"{\\\"ignoreDuplicates\\\": \\\"false\\\", \\\"centerReads\\\": \\\"false\\\", \\\"doExtendCustom\\\": {\\\"__current_case__\\\": 0, \\\"doExtend\\\": \\\"no\\\"}, \\\"samFlagExclude\\\": \\\"\\\", \\\"skipZeros\\\": \\\"false\\\", \\\"binSize\\\": \\\"500\\\", \\\"numberOfSamples\\\": \\\"100000\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"plotTitle\\\": \\\"\\\", \\\"samFlagInclude\\\": \\\"\\\", \\\"minMappingQuality\\\": \\\"1\\\"}\", \"region\": \"\\\"\\\"\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "8e092a76-27e1-4f77-9e0e-512140f9cbb8", 
            "workflow_outputs": []
        }, 
        "23": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_MarkDuplicates/1.136.0", 
            "id": 23, 
            "input_connections": {
                "inputFile": {
                    "id": 17, 
                    "output_name": "output1"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool MarkDuplicates", 
                    "name": "inputFile"
                }
            ], 
            "label": null, 
            "name": "MarkDuplicates", 
            "outputs": [
                {
                    "name": "metrics_file", 
                    "type": "txt"
                }, 
                {
                    "name": "outFile", 
                    "type": "bam"
                }
            ], 
            "position": {
                "left": 1163.5833740234375, 
                "top": 1529
            }, 
            "post_job_actions": {
                "HideDatasetActionmetrics_file": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "metrics_file"
                }, 
                "TagDatasetActionmetrics_file": {
                    "action_arguments": {
                        "tags": "Input-CGN-UT-rmdup"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "metrics_file"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/devteam/picard/picard_MarkDuplicates/1.136.0", 
            "tool_shed_repository": {
                "changeset_revision": "efc56ee1ade4", 
                "name": "picard", 
                "owner": "devteam", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"duplicate_scoring_strategy\": \"\\\"SUM_OF_BASE_QUALITIES\\\"\", \"remove_duplicates\": \"\\\"true\\\"\", \"read_name_regex\": \"\\\"[a-zA-Z0-9]+:[0-9]:([0-9]+):([0-9]+):([0-9]+).*.\\\"\", \"__page__\": 0, \"__rerun_remap_job_id__\": null, \"optical_duplicate_pixel_distance\": \"\\\"100\\\"\", \"comments\": \"[]\", \"assume_sorted\": \"\\\"false\\\"\", \"validation_stringency\": \"\\\"LENIENT\\\"\", \"inputFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "1.136.0", 
            "type": "tool", 
            "uuid": "c4ccef0a-a401-4a0b-9206-8d50952541f8", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFile", 
                    "uuid": "8d85b1c5-287f-4181-9d11-c9601a0f246a"
                }
            ]
        }, 
        "24": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_bam_coverage/deeptools_bam_coverage/2.2.3.0", 
            "id": 24, 
            "input_connections": {
                "bamInput": {
                    "id": 20, 
                    "output_name": "outFile"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool bamCoverage", 
                    "name": "bamInput"
                }
            ], 
            "label": null, 
            "name": "bamCoverage", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "bigwig"
                }
            ], 
            "position": {
                "left": 1768.25, 
                "top": 635.75
            }, 
            "post_job_actions": {
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "ChIP-CGN-UT"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_bam_coverage/deeptools_bam_coverage/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "65e0795278b4", 
                "name": "deeptools_bam_coverage", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"outFileFormat\": \"\\\"bigwig\\\"\", \"region\": \"\\\"\\\"\", \"bamInput\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"binSize\": \"\\\"50\\\"\", \"scaling\": \"{\\\"effectiveGenomeSize\\\": {\\\"effectiveGenomeSize_opt\\\": \\\"2150570000\\\", \\\"__current_case__\\\": 1}, \\\"type\\\": \\\"1x\\\", \\\"scaleFactor\\\": \\\"1.0\\\", \\\"__current_case__\\\": 2}\", \"advancedOpt\": \"{\\\"ignoreDuplicates\\\": \\\"false\\\", \\\"centerReads\\\": \\\"false\\\", \\\"doExtendCustom\\\": {\\\"__current_case__\\\": 0, \\\"doExtend\\\": \\\"no\\\"}, \\\"samFlagExclude\\\": \\\"\\\", \\\"samFlagInclude\\\": \\\"\\\", \\\"filterRNAstrand\\\": \\\"no\\\", \\\"smoothLength\\\": \\\"\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"MNase\\\": \\\"false\\\", \\\"ignoreForNormalization\\\": \\\"\\\", \\\"skipNAs\\\": \\\"false\\\", \\\"minMappingQuality\\\": \\\"1\\\"}\", \"__rerun_remap_job_id__\": null}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "d7378626-53cb-4b12-97c5-d796066712f0", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "077e2b9f-dd8c-41b7-b11e-326bf66a24bf"
                }
            ]
        }, 
        "25": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/iuc/macs2/macs2_callpeak/2.1.0.20140616.0", 
            "id": 25, 
            "input_connections": {
                "input_control_file": {
                    "id": 23, 
                    "output_name": "outFile"
                }, 
                "input_treatment_file": {
                    "id": 20, 
                    "output_name": "outFile"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool MACS2 callpeak", 
                    "name": "input_control_file"
                }, 
                {
                    "description": "runtime parameter for tool MACS2 callpeak", 
                    "name": "input_treatment_file"
                }
            ], 
            "label": null, 
            "name": "MACS2 callpeak", 
            "outputs": [
                {
                    "name": "output_bed", 
                    "type": "bed"
                }, 
                {
                    "name": "output_broadpeaks", 
                    "type": "bed"
                }, 
                {
                    "name": "output_gappedpeaks", 
                    "type": "tabular"
                }, 
                {
                    "name": "output_narrowpeaks", 
                    "type": "tabular"
                }, 
                {
                    "name": "output_summits", 
                    "type": "bed"
                }, 
                {
                    "name": "output_plot", 
                    "type": "pdf"
                }, 
                {
                    "name": "output_treat_pileup", 
                    "type": "bedgraph"
                }, 
                {
                    "name": "output_control_lambda", 
                    "type": "bedgraph"
                }, 
                {
                    "name": "output_extra_files", 
                    "type": "html"
                }
            ], 
            "position": {
                "left": 1764.949951171875, 
                "top": 213.51666259765625
            }, 
            "post_job_actions": {
                "HideDatasetActionoutput_control_lambda": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_control_lambda"
                }, 
                "HideDatasetActionoutput_extra_files": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_extra_files"
                }, 
                "HideDatasetActionoutput_plot": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_plot"
                }, 
                "HideDatasetActionoutput_summits": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_summits"
                }, 
                "HideDatasetActionoutput_treat_pileup": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "output_treat_pileup"
                }, 
                "TagDatasetActionoutput_bed": {
                    "action_arguments": {
                        "tags": "MACS2 callpeak (ChIP/Input)"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "output_bed"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/iuc/macs2/macs2_callpeak/2.1.0.20140616.0", 
            "tool_shed_repository": {
                "changeset_revision": "859c982b1f7f", 
                "name": "macs2", 
                "owner": "iuc", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"effective_genome_size_options\": \"{\\\"effective_genome_size_options_selector\\\": \\\"2150570000\\\", \\\"__current_case__\\\": 2}\", \"bampe\": \"\\\"true\\\"\", \"input_control_file\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__rerun_remap_job_id__\": null, \"outputs\": \"[\\\"peaks_bed\\\", \\\"summits\\\", \\\"bdg\\\", \\\"html\\\"]\", \"cutoff_options\": \"{\\\"cutoff_options_selector\\\": \\\"qvalue\\\", \\\"qvalue\\\": \\\"0.05\\\", \\\"__current_case__\\\": 1}\", \"advanced_options\": \"{\\\"advanced_options_selector\\\": \\\"on\\\", \\\"ratio\\\": \\\"1.0\\\", \\\"to_large\\\": \\\"false\\\", \\\"slocal\\\": \\\"1000\\\", \\\"broad_options\\\": {\\\"broad_options_selector\\\": \\\"nobroad\\\", \\\"call_summits\\\": \\\"false\\\", \\\"__current_case__\\\": 1}, \\\"nolambda\\\": \\\"false\\\", \\\"llocal\\\": \\\"10000\\\", \\\"keep_dup_options\\\": {\\\"__current_case__\\\": 1, \\\"keep_dup_options_selector\\\": \\\"1\\\"}, \\\"__current_case__\\\": 0}\", \"input_treatment_file\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"nomodel_type\": \"{\\\"nomodel_type_selector\\\": \\\"create_model\\\", \\\"__current_case__\\\": 0}\", \"band_width\": \"\\\"300\\\"\"}", 
            "tool_version": "2.1.0.20140616.0", 
            "type": "tool", 
            "uuid": "0a211107-481f-4ac3-9701-5acde7e53e9a", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "output_gappedpeaks", 
                    "uuid": "11b11ba2-5936-491e-93f1-156b60907933"
                }, 
                {
                    "label": null, 
                    "output_name": "output_broadpeaks", 
                    "uuid": "b1ef3abd-a5b3-4b58-83ca-a8d933734ea5"
                }, 
                {
                    "label": null, 
                    "output_name": "output_bed", 
                    "uuid": "ab69c7e3-3eb4-4595-ae94-90a053946379"
                }, 
                {
                    "label": null, 
                    "output_name": "output_narrowpeaks", 
                    "uuid": "863b7a25-0b27-4c8d-80b9-821403ad6400"
                }
            ]
        }, 
        "26": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_bam_compare/deeptools_bam_compare/2.2.3.0", 
            "id": 26, 
            "input_connections": {
                "bamFile1": {
                    "id": 20, 
                    "output_name": "outFile"
                }, 
                "bamFile2": {
                    "id": 23, 
                    "output_name": "outFile"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool bamCompare", 
                    "name": "bamFile2"
                }, 
                {
                    "description": "runtime parameter for tool bamCompare", 
                    "name": "bamFile1"
                }
            ], 
            "label": null, 
            "name": "bamCompare", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "bigwig"
                }
            ], 
            "position": {
                "left": 1762.25, 
                "top": 863.75
            }, 
            "post_job_actions": {}, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_bam_compare/deeptools_bam_compare/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "d5d57b40b29a", 
                "name": "deeptools_bam_compare", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"comparison\": \"{\\\"pseudocount\\\": \\\"1.0\\\", \\\"type\\\": \\\"log2\\\", \\\"__current_case__\\\": 0}\", \"bamFile2\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"outFileFormat\": \"\\\"bigwig\\\"\", \"bamFile1\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"__page__\": 0, \"region\": \"\\\"\\\"\", \"binSize\": \"\\\"50\\\"\", \"scaling\": \"{\\\"method\\\": \\\"readCount\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"showAdvancedOpt\\\": \\\"no\\\", \\\"__current_case__\\\": 0}\", \"__rerun_remap_job_id__\": null}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "7cfd9cce-e343-4c30-a87f-250ee88ab5a4", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "0bbe0aec-b562-4d74-ba30-74ffd0d25abe"
                }
            ]
        }, 
        "27": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_bam_coverage/deeptools_bam_coverage/2.2.3.0", 
            "id": 27, 
            "input_connections": {
                "bamInput": {
                    "id": 23, 
                    "output_name": "outFile"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool bamCoverage", 
                    "name": "bamInput"
                }
            ], 
            "label": null, 
            "name": "bamCoverage", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "bigwig"
                }
            ], 
            "position": {
                "left": 1776.25, 
                "top": 1190.75
            }, 
            "post_job_actions": {
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "Input-CGN-UT"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_bam_coverage/deeptools_bam_coverage/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "65e0795278b4", 
                "name": "deeptools_bam_coverage", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"outFileFormat\": \"\\\"bigwig\\\"\", \"region\": \"\\\"\\\"\", \"bamInput\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"binSize\": \"\\\"50\\\"\", \"scaling\": \"{\\\"effectiveGenomeSize\\\": {\\\"effectiveGenomeSize_opt\\\": \\\"2150570000\\\", \\\"__current_case__\\\": 1}, \\\"type\\\": \\\"1x\\\", \\\"scaleFactor\\\": \\\"1.0\\\", \\\"__current_case__\\\": 2}\", \"advancedOpt\": \"{\\\"ignoreDuplicates\\\": \\\"false\\\", \\\"centerReads\\\": \\\"false\\\", \\\"doExtendCustom\\\": {\\\"__current_case__\\\": 0, \\\"doExtend\\\": \\\"no\\\"}, \\\"samFlagExclude\\\": \\\"\\\", \\\"samFlagInclude\\\": \\\"\\\", \\\"filterRNAstrand\\\": \\\"no\\\", \\\"smoothLength\\\": \\\"\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"MNase\\\": \\\"false\\\", \\\"ignoreForNormalization\\\": \\\"\\\", \\\"skipNAs\\\": \\\"false\\\", \\\"minMappingQuality\\\": \\\"1\\\"}\", \"__rerun_remap_job_id__\": null}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "56d01d68-f0b6-4849-9aeb-a0a9f7779905", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "83343b5a-0c47-4805-bd91-bd10cc32166a"
                }
            ]
        }, 
        "28": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "id": 28, 
            "input_connections": {
                "regionsFiles_0|regionsFile": {
                    "id": 4, 
                    "output_name": "output"
                }, 
                "scoreFileName": {
                    "id": 24, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool computeMatrix", 
                    "name": "scoreFileName"
                }
            ], 
            "label": null, 
            "name": "computeMatrix", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "deeptools_compute_matrix_archive"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2264.25, 
                "top": 566.75
            }, 
            "post_job_actions": {}, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "17d456f4051b", 
                "name": "deeptools_compute_matrix", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"mode\": \"{\\\"regionBodyLength\\\": \\\"4000\\\", \\\"regionStartLength\\\": {\\\"afterRegionStartLength\\\": \\\"2000\\\", \\\"unscaled5prime\\\": \\\"0\\\", \\\"beforeRegionStartLength\\\": \\\"2000\\\", \\\"regionStartLength_select\\\": \\\"yes\\\", \\\"unscaled3prime\\\": \\\"0\\\", \\\"__current_case__\\\": 1}, \\\"__current_case__\\\": 0, \\\"mode_select\\\": \\\"scale-regions\\\"}\", \"scoreFileName\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"saveSortedRegions\\\": \\\"false\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"averageTypeBins\\\": \\\"mean\\\", \\\"maxThreshold\\\": \\\"\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"skipZeros\\\": \\\"false\\\", \\\"binSize\\\": \\\"10\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"scale\\\": \\\"\\\", \\\"__current_case__\\\": 1, \\\"minThreshold\\\": \\\"\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"missingDataAsZero\\\": \\\"false\\\"}\", \"regionsFiles\": \"[{\\\"__index__\\\": 0, \\\"regionsFile\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}}]\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "1f76d0bb-8043-48fc-9576-b5fdf5f750e9", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "34eb8c5e-3014-45a9-b4e5-0a9e4a49093d"
                }, 
                {
                    "label": null, 
                    "output_name": "outFileNameMatrix", 
                    "uuid": "659518b8-243b-4e37-aae2-48248e9b3eee"
                }, 
                {
                    "label": null, 
                    "output_name": "outFileSortedRegions", 
                    "uuid": "33366276-be13-4651-968e-691095107a60"
                }
            ]
        }, 
        "29": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "id": 29, 
            "input_connections": {
                "regionsFiles_0|regionsFile": {
                    "id": 25, 
                    "output_name": "output_bed"
                }, 
                "scoreFileName": {
                    "id": 4, 
                    "output_name": "output"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool computeMatrix", 
                    "name": "scoreFileName"
                }
            ], 
            "label": null, 
            "name": "computeMatrix", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "deeptools_compute_matrix_archive"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2266.25, 
                "top": 287.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileNameMatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileNameMatrix"
                }, 
                "HideDatasetActionoutFileSortedRegions": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileSortedRegions"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "17d456f4051b", 
                "name": "deeptools_compute_matrix", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"mode\": \"{\\\"regionBodyLength\\\": \\\"4000\\\", \\\"regionStartLength\\\": {\\\"afterRegionStartLength\\\": \\\"2000\\\", \\\"unscaled5prime\\\": \\\"0\\\", \\\"beforeRegionStartLength\\\": \\\"2000\\\", \\\"regionStartLength_select\\\": \\\"yes\\\", \\\"unscaled3prime\\\": \\\"0\\\", \\\"__current_case__\\\": 1}, \\\"__current_case__\\\": 0, \\\"mode_select\\\": \\\"scale-regions\\\"}\", \"scoreFileName\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"saveSortedRegions\\\": \\\"false\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"averageTypeBins\\\": \\\"mean\\\", \\\"maxThreshold\\\": \\\"\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"skipZeros\\\": \\\"false\\\", \\\"binSize\\\": \\\"10\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"scale\\\": \\\"\\\", \\\"__current_case__\\\": 1, \\\"minThreshold\\\": \\\"\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"missingDataAsZero\\\": \\\"false\\\"}\", \"regionsFiles\": \"[{\\\"__index__\\\": 0, \\\"regionsFile\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}}]\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "c1b07f2e-1050-49d9-a8f0-ab40aa06ab1c", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "3efa6012-32ea-4da6-a053-4283f7263e3c"
                }
            ]
        }, 
        "30": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "id": 30, 
            "input_connections": {
                "regionsFiles_0|regionsFile": {
                    "id": 4, 
                    "output_name": "output"
                }, 
                "scoreFileName": {
                    "id": 26, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool computeMatrix", 
                    "name": "scoreFileName"
                }
            ], 
            "label": null, 
            "name": "computeMatrix", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "deeptools_compute_matrix_archive"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2265.25, 
                "top": 873.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileNameMatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileNameMatrix"
                }, 
                "HideDatasetActionoutFileSortedRegions": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileSortedRegions"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "17d456f4051b", 
                "name": "deeptools_compute_matrix", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"mode\": \"{\\\"regionBodyLength\\\": \\\"4000\\\", \\\"regionStartLength\\\": {\\\"afterRegionStartLength\\\": \\\"2000\\\", \\\"unscaled5prime\\\": \\\"0\\\", \\\"beforeRegionStartLength\\\": \\\"2000\\\", \\\"regionStartLength_select\\\": \\\"yes\\\", \\\"unscaled3prime\\\": \\\"0\\\", \\\"__current_case__\\\": 1}, \\\"__current_case__\\\": 0, \\\"mode_select\\\": \\\"scale-regions\\\"}\", \"scoreFileName\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"output\": \"{\\\"showOutputSettings\\\": \\\"no\\\", \\\"__current_case__\\\": 0}\", \"advancedOpt\": \"{\\\"averageTypeBins\\\": \\\"mean\\\", \\\"maxThreshold\\\": \\\"\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"skipZeros\\\": \\\"false\\\", \\\"binSize\\\": \\\"10\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"scale\\\": \\\"\\\", \\\"__current_case__\\\": 1, \\\"minThreshold\\\": \\\"\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"missingDataAsZero\\\": \\\"false\\\"}\", \"regionsFiles\": \"[{\\\"__index__\\\": 0, \\\"regionsFile\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}}]\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "bbdb24cf-36b5-4fd6-87e2-986a286df995", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "a11cdb4d-d4bc-4fde-9cd8-3d10f325ddc4"
                }
            ]
        }, 
        "31": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "id": 31, 
            "input_connections": {
                "regionsFiles_0|regionsFile": {
                    "id": 4, 
                    "output_name": "output"
                }, 
                "scoreFileName": {
                    "id": 27, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool computeMatrix", 
                    "name": "scoreFileName"
                }
            ], 
            "label": null, 
            "name": "computeMatrix", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "deeptools_compute_matrix_archive"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2266.25, 
                "top": 1200.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileNameMatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileNameMatrix"
                }, 
                "HideDatasetActionoutFileSortedRegions": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileSortedRegions"
                }, 
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "UCSC/bamCoverage (Input)"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_compute_matrix/deeptools_compute_matrix/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "17d456f4051b", 
                "name": "deeptools_compute_matrix", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"__rerun_remap_job_id__\": null, \"mode\": \"{\\\"regionBodyLength\\\": \\\"4000\\\", \\\"regionStartLength\\\": {\\\"afterRegionStartLength\\\": \\\"2000\\\", \\\"unscaled5prime\\\": \\\"0\\\", \\\"beforeRegionStartLength\\\": \\\"2000\\\", \\\"regionStartLength_select\\\": \\\"yes\\\", \\\"unscaled3prime\\\": \\\"0\\\", \\\"__current_case__\\\": 1}, \\\"__current_case__\\\": 0, \\\"mode_select\\\": \\\"scale-regions\\\"}\", \"scoreFileName\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\", \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"saveSortedRegions\\\": \\\"true\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"averageTypeBins\\\": \\\"mean\\\", \\\"maxThreshold\\\": \\\"\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"skipZeros\\\": \\\"true\\\", \\\"binSize\\\": \\\"10\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"scale\\\": \\\"\\\", \\\"__current_case__\\\": 1, \\\"minThreshold\\\": \\\"10.0\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"missingDataAsZero\\\": \\\"false\\\"}\", \"regionsFiles\": \"[{\\\"__index__\\\": 0, \\\"regionsFile\\\": {\\\"__class__\\\": \\\"RuntimeValue\\\"}}]\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "cce6bee2-731b-45e7-9c60-ae469f0b5c2d", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "01fbbb6d-e943-4ead-baf9-275ae4bab92d"
                }
            ]
        }, 
        "32": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "id": 32, 
            "input_connections": {
                "matrixFile": {
                    "id": 28, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool plotHeatmap", 
                    "name": "matrixFile"
                }
            ], 
            "label": null, 
            "name": "plotHeatmap", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "png"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2600.25, 
                "top": 583.75
            }, 
            "post_job_actions": {
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "UCSC/bamCoverage (ChIP)"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "e57bfadcab30", 
                "name": "deeptools_plot_heatmap", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"outFileFormat\\\": \\\"png\\\", \\\"saveSortedRegions\\\": \\\"true\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"used_multiple_regions\\\": {\\\"__current_case__\\\": 1, \\\"used_multiple_regions_options\\\": \\\"yes\\\"}, \\\"yAxisLabel\\\": \\\"genes\\\", \\\"xAxisLabel\\\": \\\"distance from TSS (bp)\\\", \\\"perGroup\\\": \\\"false\\\", \\\"zMax\\\": \\\"\\\", \\\"heatmapWidth\\\": \\\"7.5\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"zMin\\\": \\\"\\\", \\\"plotTitle\\\": \\\"\\\", \\\"averageTypeSummaryPlot\\\": \\\"mean\\\", \\\"whatToShow\\\": \\\"plot, heatmap and colorbar\\\", \\\"missingDataColor\\\": \\\"black\\\", \\\"referencePointLabel\\\": \\\"TSS\\\", \\\"yMin\\\": \\\"\\\", \\\"regionsLabel\\\": \\\"\\\", \\\"yMax\\\": \\\"\\\", \\\"samplesLabel\\\": \\\"\\\", \\\"endLabel\\\": \\\"TES\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"startLabel\\\": \\\"TSS\\\", \\\"colorMap\\\": \\\"RdYlBu\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"heatmapHeight\\\": \\\"25.0\\\"}\", \"__rerun_remap_job_id__\": null, \"matrixFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "a48e93d9-d93a-47e8-a76e-4748545bcfca", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "77a9e9cf-475c-4c08-8adb-00ca68ae7417"
                }, 
                {
                    "label": null, 
                    "output_name": "outFileNameMatrix", 
                    "uuid": "78e6806e-f58c-4a5a-87b7-f5ffdbe3e27b"
                }, 
                {
                    "label": null, 
                    "output_name": "outFileSortedRegions", 
                    "uuid": "55b5a083-0dfa-403d-bf8a-44e459cb48bf"
                }
            ]
        }, 
        "33": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "id": 33, 
            "input_connections": {
                "matrixFile": {
                    "id": 29, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool plotHeatmap", 
                    "name": "matrixFile"
                }
            ], 
            "label": null, 
            "name": "plotHeatmap", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "png"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2596.25, 
                "top": 311.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileNameMatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileNameMatrix"
                }, 
                "HideDatasetActionoutFileSortedRegions": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileSortedRegions"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "e57bfadcab30", 
                "name": "deeptools_plot_heatmap", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"outFileFormat\\\": \\\"png\\\", \\\"saveSortedRegions\\\": \\\"true\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"used_multiple_regions\\\": {\\\"__current_case__\\\": 1, \\\"used_multiple_regions_options\\\": \\\"yes\\\"}, \\\"yAxisLabel\\\": \\\"genes\\\", \\\"xAxisLabel\\\": \\\"distance from TSS (bp)\\\", \\\"perGroup\\\": \\\"false\\\", \\\"zMax\\\": \\\"\\\", \\\"heatmapWidth\\\": \\\"7.5\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"zMin\\\": \\\"\\\", \\\"plotTitle\\\": \\\"\\\", \\\"averageTypeSummaryPlot\\\": \\\"mean\\\", \\\"whatToShow\\\": \\\"plot, heatmap and colorbar\\\", \\\"missingDataColor\\\": \\\"black\\\", \\\"referencePointLabel\\\": \\\"TSS\\\", \\\"yMin\\\": \\\"\\\", \\\"regionsLabel\\\": \\\"\\\", \\\"yMax\\\": \\\"\\\", \\\"samplesLabel\\\": \\\"\\\", \\\"endLabel\\\": \\\"TES\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"startLabel\\\": \\\"TSS\\\", \\\"colorMap\\\": \\\"RdYlBu\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"heatmapHeight\\\": \\\"25.0\\\"}\", \"__rerun_remap_job_id__\": null, \"matrixFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "7b6db088-92ba-416c-88f5-38169a0abf44", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "6cef8e79-b961-4d7a-817b-1c8941594af1"
                }
            ]
        }, 
        "34": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "id": 34, 
            "input_connections": {
                "matrixFile": {
                    "id": 30, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool plotHeatmap", 
                    "name": "matrixFile"
                }
            ], 
            "label": null, 
            "name": "plotHeatmap", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "png"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2602.25, 
                "top": 891.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileNameMatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileNameMatrix"
                }, 
                "HideDatasetActionoutFileSortedRegions": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileSortedRegions"
                }, 
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "UCSC/bamCompare (ChIP/Input)"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "e57bfadcab30", 
                "name": "deeptools_plot_heatmap", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"outFileFormat\\\": \\\"png\\\", \\\"saveSortedRegions\\\": \\\"true\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"used_multiple_regions\\\": {\\\"__current_case__\\\": 1, \\\"used_multiple_regions_options\\\": \\\"yes\\\"}, \\\"yAxisLabel\\\": \\\"genes\\\", \\\"xAxisLabel\\\": \\\"distance from TSS (bp)\\\", \\\"perGroup\\\": \\\"false\\\", \\\"zMax\\\": \\\"\\\", \\\"heatmapWidth\\\": \\\"7.5\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"zMin\\\": \\\"\\\", \\\"plotTitle\\\": \\\"\\\", \\\"averageTypeSummaryPlot\\\": \\\"mean\\\", \\\"whatToShow\\\": \\\"plot, heatmap and colorbar\\\", \\\"missingDataColor\\\": \\\"black\\\", \\\"referencePointLabel\\\": \\\"TSS\\\", \\\"yMin\\\": \\\"\\\", \\\"regionsLabel\\\": \\\"\\\", \\\"yMax\\\": \\\"\\\", \\\"samplesLabel\\\": \\\"\\\", \\\"endLabel\\\": \\\"TES\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"startLabel\\\": \\\"TSS\\\", \\\"colorMap\\\": \\\"RdYlBu\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"heatmapHeight\\\": \\\"25.0\\\"}\", \"__rerun_remap_job_id__\": null, \"matrixFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "0d0c7d69-8d30-4e30-88d0-7f57efe67210", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "b423c06a-3013-4dfe-8da9-e775e1570964"
                }
            ]
        }, 
        "35": {
            "annotation": "", 
            "content_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "id": 35, 
            "input_connections": {
                "matrixFile": {
                    "id": 31, 
                    "output_name": "outFileName"
                }
            }, 
            "inputs": [
                {
                    "description": "runtime parameter for tool plotHeatmap", 
                    "name": "matrixFile"
                }
            ], 
            "label": null, 
            "name": "plotHeatmap", 
            "outputs": [
                {
                    "name": "outFileName", 
                    "type": "png"
                }, 
                {
                    "name": "outFileSortedRegions", 
                    "type": "bed"
                }, 
                {
                    "name": "outFileNameMatrix", 
                    "type": "tabular"
                }
            ], 
            "position": {
                "left": 2605.25, 
                "top": 1212.75
            }, 
            "post_job_actions": {
                "HideDatasetActionoutFileNameMatrix": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileNameMatrix"
                }, 
                "HideDatasetActionoutFileSortedRegions": {
                    "action_arguments": {}, 
                    "action_type": "HideDatasetAction", 
                    "output_name": "outFileSortedRegions"
                }, 
                "TagDatasetActionoutFileName": {
                    "action_arguments": {
                        "tags": "UCSC/bamCoverage (Input)"
                    }, 
                    "action_type": "TagDatasetAction", 
                    "output_name": "outFileName"
                }
            }, 
            "tool_errors": null, 
            "tool_id": "toolshed.g2.bx.psu.edu/repos/bgruening/deeptools_plot_heatmap/deeptools_plot_heatmap/2.2.3.0", 
            "tool_shed_repository": {
                "changeset_revision": "e57bfadcab30", 
                "name": "deeptools_plot_heatmap", 
                "owner": "bgruening", 
                "tool_shed": "toolshed.g2.bx.psu.edu"
            }, 
            "tool_state": "{\"__page__\": 0, \"output\": \"{\\\"saveMatrix\\\": \\\"false\\\", \\\"outFileFormat\\\": \\\"png\\\", \\\"saveSortedRegions\\\": \\\"false\\\", \\\"showOutputSettings\\\": \\\"yes\\\", \\\"__current_case__\\\": 1}\", \"advancedOpt\": \"{\\\"used_multiple_regions\\\": {\\\"__current_case__\\\": 1, \\\"used_multiple_regions_options\\\": \\\"yes\\\"}, \\\"yAxisLabel\\\": \\\"genes\\\", \\\"xAxisLabel\\\": \\\"distance from TSS (bp)\\\", \\\"perGroup\\\": \\\"false\\\", \\\"zMax\\\": \\\"\\\", \\\"heatmapWidth\\\": \\\"7.5\\\", \\\"sortUsing\\\": \\\"mean\\\", \\\"zMin\\\": \\\"\\\", \\\"plotTitle\\\": \\\"\\\", \\\"averageTypeSummaryPlot\\\": \\\"mean\\\", \\\"whatToShow\\\": \\\"plot, heatmap and colorbar\\\", \\\"missingDataColor\\\": \\\"black\\\", \\\"referencePointLabel\\\": \\\"TSS\\\", \\\"yMin\\\": \\\"\\\", \\\"regionsLabel\\\": \\\"\\\", \\\"yMax\\\": \\\"\\\", \\\"samplesLabel\\\": \\\"\\\", \\\"endLabel\\\": \\\"TES\\\", \\\"sortRegions\\\": \\\"descend\\\", \\\"startLabel\\\": \\\"TSS\\\", \\\"colorMap\\\": \\\"RdYlBu\\\", \\\"showAdvancedOpt\\\": \\\"yes\\\", \\\"__current_case__\\\": 1, \\\"heatmapHeight\\\": \\\"25.0\\\"}\", \"__rerun_remap_job_id__\": null, \"matrixFile\": \"{\\\"__class__\\\": \\\"RuntimeValue\\\"}\"}", 
            "tool_version": "2.2.3.0", 
            "type": "tool", 
            "uuid": "ff8d50e9-1d41-4645-98e3-9bd70cca93e4", 
            "workflow_outputs": [
                {
                    "label": null, 
                    "output_name": "outFileName", 
                    "uuid": "e9e8734b-7942-4666-95f5-4ccb3946c8d0"
                }
            ]
        }
    }, 
    "uuid": "e76c7ea5-f361-4923-83ce-731726e8046b"
}
