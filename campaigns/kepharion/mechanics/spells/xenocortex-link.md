- name:: : [[Xenocortex]] Link
- level:: : 2
- school:: Divination
- casting_time:: 1 action
- range:: Touch
- components:: V, S, M (a small crystal resonator)
- duration:: Concentration, up to 10 minutes
- classes:: Singer, Symphonist
- campaign:: : [[kepharion]]
- source:: [[Kepharion]] Campaign
- xenocortex_spell:: true
- last_updated:: 2025-07-02T18:00:00Z

- # [[Xenocortex]] Link

- *2nd-level divination*

- **Casting Time:** 1 action
- **Range:** Touch
- **Components:** V, S, M (a small crystal resonator)
- **Duration:** Concentration, up to 10 minutes
- **Classes:** Singer, Symphonist

- You create a temporary mental link between your [[xenocortex]] and that of a willing Vaarn creature you touch. For the duration, you and the target can communicate telepathically and share certain mental resources.

- ## Effects

- ### Telepathic Communication
- Both participants can communicate telepathically regardless of language barriers
- Communication range extends up to 1 mile
- Emotional context is automatically shared along with thoughts
- Either participant can choose to block specific thoughts from sharing

- ### Pattern Sharing
- You can access each other's stored [[xenocortex]] patterns
- Each participant can use one of the other's stored patterns per turn
- Shared patterns are used from the original owner's daily limit
- Complex patterns may require both participants to coordinate for full effect

- ### Enhanced Processing
- When working on the same mental task, both participants gain advantage on Intelligence-based checks
- Memory searches become much more efficient when conducted jointly
- Problem-solving benefits from dual perspective analysis
- Creative tasks gain inspiration bonus from shared consciousness

- ### Harmonic Resonance
- Both participants become attuned to each other's emotional state
- Advantage on saving throws against fear and charm effects while linked
- Can share the benefits of successful saving throws with linked partner
- Emotional stability is enhanced through shared mental strength

- ## At Higher Levels

- **3rd Level:** Duration increases to 1 hour, and you can include one additional willing Vaarn in the link.

- **4th Level:** Duration increases to 8 hours, and the link can include up to 3 additional willing Vaarn.

- **5th Level:** Duration becomes 24 hours, and you can create a permanent version of this spell that lasts until dispelled. A permanent link can include up to 5 willing Vaarn and allows for much deeper sharing of memories, skills, and [[xenocortex]] capabilities.

- ## Risks and Limitations

- ### Mental Strain
- If either participant takes psychic damage, both must make a Constitution saving throw or suffer half the damage
- Overuse of shared patterns can cause temporary [[xenocortex]] exhaustion
- Maintaining the link for the full duration requires concentration checks when taking damage

- ### Privacy Concerns
- Intense emotions or traumatic memories may leak through the link involuntarily
- Participants must trust each other completely, as deception becomes nearly impossible
- Breaking the link abruptly (such as through counterspell) causes 1d6 psychic damage to both participants

- ### Cultural Implications
- In Nuvarden society, unauthorized [[xenocortex]] linking is considered a serious religious violation
- Alossi culture treats this as an experimental procedure requiring proper safety protocols
- Tazun communities often incorporate such links into artistic and cultural ceremonies

- ## Spell Components

- ### Verbal Component
		- A harmonic frequency that resonates with [[xenocortex]] crystals, typically hummed or chanted in a specific pattern that synchronizes the participants' neural oscillations.

- ### Somatic Component
		- Specific hand positions that create geometric patterns corresponding to [[xenocortex]] lattice structures, helping to establish the mental connection.

- ### Material Component
		- A small crystal resonator attuned to [[xenocortex]] frequencies. The crystal must be held by both participants during the initial casting and glows faintly while the link is active.

- ## AI Behavior Modifications

- ```ruby
- def xenocortex_link_decision_making(linked_characters)
- # Linked characters share decision confidence and can coordinate responses
- shared_confidence = linked_characters.map(&:decision_confidence).max
  
- linked_characters.each do |character|
- character[:ai_traits][:coordination] *= 1.5
- character[:ai_traits][:shared_processing] = 2.0
- character[:decision_confidence] = shared_confidence
- end
  
- return coordinate_linked_actions(linked_characters)
- end

- def pattern_sharing_optimization(participant_a, participant_b, task_type)
- available_patterns = participant_a[:stored_patterns] + participant_b[:stored_patterns]
- optimal_patterns = select_best_patterns_for_task(available_patterns, task_type)
  
- return distribute_pattern_usage(optimal_patterns, [participant_a, participant_b])
- end
- ```

- ## Related Mechanics
- [[xenocortex]]-pattern-storage]] - Rules for sharing stored patterns
- [[telepathic-communication]] - Guidelines for mental communication
- [[vaarn-mental-linking]] - Cultural and social implications of mental links