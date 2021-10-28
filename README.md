	</launch>

name="auto_sort" default="false"/>
  <arg name="at_dock" default="false"/>
  <arg name="gripper_open" default="0.031"/>
  <arg name="block_size" default="0.02"/>
  <arg name="gripper_tighten" default="0.004"/>
  <arg name="z_up" default="0.06"/>
  <arg name="target_bin_height" default="0.06"/>
  <arg name="table_height" default="0.0"/>
  <arg name="auto_sort" default="false"/>

  <include file="$(find turtlebot2i_block_manipulation)/launch/block_manipulation.launch">
    <arg name="at_dock" value="$(arg at_dock)"/>
  </include>

  <node name="block_manipulation_demo" pkg="turtlebot2i_block_manipulation" type="block_manipulation_demo" output="screen" >
    <param name="arm_link" value="/arm_base_link" />
    <param name="gripper_open" value="0.031" />
    <param name="gripper_open" value="$(arg gripper_open)" />
    <param name="block_size" value="$(arg block_size)" />
    <param name="gripper_tighten" value="0.004" />
    <param name="z_up" value="0.06" />
    <param name="target_bin_height" value="0.06" />
    <param name="table_height" value="0.1" />

    <param name="gripper_tighten" value="$(arg gripper_tighten)" />
    <param name="z_up" value="$(arg z_up)" />
    <param name="target_bin_height" value="$(arg target_bin_height)" />
    <param name="table_height" value="$(arg table_height)" />
    <param name="auto_sort" value="$(arg auto_sort)" />

  </node>
</launch>

    <param name=
    
    
